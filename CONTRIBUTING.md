# Como contribuir com Lucy & Nero

As contribuições devem desenvolver e manter a coerência da franquia **Lucy & Nero**. São bem-vindas
melhorias de documentação, propostas narrativas, referências visuais e correções nas ferramentas.

## Referências e continuidade

Leia o [README](README.md) e as [diretrizes](AGENTS.md). As fichas [Lucy](lucy.md) e [Nero](nero.md)
preservam material anterior e não devem reintroduzir automaticamente elementos descontinuados.
Diferencie cânone, propostas, questões não definidas e conteúdo descontinuado.

## Fluxo de trabalho

Organize cada contribuição em torno de um objetivo verificável.

1. Descreva o problema ou proposta e seus critérios de aceitação. Para mudanças amplas, apresente os
   arquivos envolvidos e os impactos antes de editar.
2. Inspecione o Git e preserve o trabalho existente. Agentes seguem as regras de branch do
   AGENTS.md.
3. Faça uma mudança coesa por PR e atualize as referências afetadas.
4. Execute verificações aplicáveis, revise o diff e registre resultados e limitações reais.
5. Resolva a revisão. Alterações de cânone e merges dependem da aprovação humana.

Títulos de PR e commits seguem Conventional Commits, com até 100 caracteres e escopo opcional.
Exemplos: `docs(lore): esclarece a maturação dos Neko Ryuu` e
`fix(tooling): corrige a validação de links locais`.

## Organização do conteúdo

O README concentra a continuidade atual e a visão dos jogos. As fichas mantêm material histórico, e
public/ reúne referências visuais. Ao propor um documento novo, escolha um nome descritivo e
adicione um link no documento que o contextualiza.

Escreva em português e inclua uma descrição após cada título. Identifique spoilers, limitações,
dúvidas e decisões pendentes. Não apresente sistemas planejados como jogáveis.

## Revisão narrativa e visual

Confira a proposta contra a continuidade atual antes de solicitar revisão.

- Preserve idades, cronologia e a diferença de cinco anos entre Lucy e Nero.
- Distinga afinidade elemental, reserva de mana, domínio mágico e habilidade inata.
- Separe a maturação dos Neko Ryuu das transformações sombrias de Nero.
- Não atribua novos poderes, limites ou explicações aos personagens sem aprovação.
- Para arte, identifique personagem, forma, referência e estado de aprovação.
- Explique quais documentos precisam mudar quando uma decisão de cânone for aprovada.

## Verificações locais

O [guia das ferramentas](utils/README.md) descreve interfaces existentes e limitações. Confira a
formatação com a versão usada pelo hook:

```sh
npx --yes --package prettier@3.9.5 prettier --check README.md
```

Substitua o caminho pelos arquivos alterados. Para aplicar a formatação, use --write e revise o
resultado. Confira também links locais, âncoras do índice e descrições após os títulos.

A base usa Python 3.14+ e uv. O preparo previsto é `uv sync --locked`, seguido de
`uv run pre-commit install`. Nesta revisão, o ambiente tem uv.lock, mas ainda falta tests/; a
sequência de checks herdada ainda exige adaptação. Não altere a infraestrutura implicitamente em uma
contribuição editorial.

Antes de commitar, siga os comandos do AGENTS.md e relate falhas ou pré-requisitos ausentes. Nunca
use --no-verify nem apresente verificações não executadas como aprovadas.

## Segurança e evidências

Mudanças em validadores exigem casos aceitos, rejeitados e regressões relevantes. Use o ambiente uv
do projeto para dependências. Não inclua segredos ou dados pessoais e respeite autoria e licenças.

O sincronizador de labels ainda aponta para o repositório de origem; não o execute para administrar
Lucy & Nero antes de adaptar e revisar seu destino.

Registre no PR objetivo, arquivos, decisões, comandos executados e limitações. A revisão automática
não confirma coerência narrativa nem substitui a avaliação visual e humana.
