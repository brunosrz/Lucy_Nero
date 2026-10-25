# Ferramentas de manutenção — Lucy & Nero

Este diretório contém módulos Python de apoio à manutenção de Lucy & Nero. Os scripts foram herdados
de uma base de estudos de engenharia de software e não implementam os jogos nem validam a coerência
narrativa.

## Pré-requisitos e estado atual

O ambiente previsto usa Python 3.14+ e uv, com dependências de desenvolvimento no
[manifesto da raiz](../pyproject.toml). O manifesto ainda contém metadados da base anterior. Nesta
revisão, o ambiente tem uv.lock, mas ainda falta tests/; a sincronização bloqueada foi validada, mas
a suíte exigida pelos hooks e pelo CI precisa ser regularizada.

Não use instalação global ou pip install avulso para contornar essas pendências. Os comandos abaixo
descrevem interfaces existentes; sua listagem não representa uma execução validada.

## Validadores locais

Em um ambiente uv preparado, os validadores de commits e links oferecem estas interfaces:

| Comando                                                                            | Finalidade                         |
| ---------------------------------------------------------------------------------- | ---------------------------------- |
| `uv run python -m utils.check_commit --title "docs(lore): esclarece a cronologia"` | Validar título de PR               |
| `uv run python -m utils.check_commit .git/COMMIT_EDITMSG`                          | Validar mensagem de commit         |
| `uv run python -m utils.check_links README.md CONTRIBUTING.md`                     | Verificar destinos locais de links |

O validador de commits aceita os tipos do AGENTS.md, escopo opcional e títulos de até 100
caracteres. Ele não avalia a precisão da descrição.

O verificador de links cobre links inline relativos, ignora blocos de código, âncoras e URLs
externas; não valida IDs de títulos nem links por referência. Não faz requisições de rede. Confira o
índice e os links externos separadamente.

## Descoberta de projetos herdada

O módulo utils.projects ainda procura manifestos nas pastas python/, go/, rust/, ts/ e cpp/. Essa
convenção vem da base anterior e não define a organização dos jogos.

| Comando                                    | Comportamento atual                            |
| ------------------------------------------ | ---------------------------------------------- |
| `uv run python -m utils.projects discover` | Lista projetos encontrados nas pastas herdadas |
| `uv run python -m utils.projects check`    | Executa verificações dos projetos descobertos  |

Diretórios gerados são ignorados e workspaces aninhados usam o manifesto mais externo. Ferramentas
ausentes geram falha; o runner verifica ausência de testes em Python e C++. Sem projetos
descobertos, não há testes de gameplay: um resultado sem erros não comprova que Little Garden, As
Crônicas de Nero ou Entre Espadas e Garras estejam implementados.

## Sincronização de labels pendente de adaptação

O módulo utils.sync_labels lê o [catálogo de labels](../.github/labels.json) e usa o GitHub CLI para
criar ou atualizar labels. Seu destino está fixado em brunosrz/src, o repositório de origem. Não o
execute para administrar Lucy & Nero antes de adaptar e revisar o destino e o catálogo. Essa
operação modifica dados remotos e exige autorização para o repositório correto.

## Limitações e manutenção

Hooks e workflows preservam referências à organização por estudos. A adaptação desta documentação
não altera esses scripts nem comprova o funcionamento do CI.

Ao mudar um validador, cubra entradas aceitas, rejeitadas e regressões. Registre comandos e
resultados reais, sem esconder falhas por dependências ou ferramentas ausentes. Consulte o
[guia de contribuição](../CONTRIBUTING.md) e as [diretrizes de agentes](../AGENTS.md).
