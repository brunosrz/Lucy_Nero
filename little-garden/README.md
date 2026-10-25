# 🌸 Lucy & Nero — Little Garden

Este documento reúne a concepção narrativa e as propostas de estrutura jogável de Little Garden,
primeiro lançamento planejado da franquia **Lucy & Nero**.

> **Documento de concepção e estrutura do jogo (GDD + bíblia narrativa)**
>
> **Uso:** repositório privado; contém spoilers da franquia.
>
> **Situação:** primeiro jogo planejado para lançamento no universo Lucy & Nero.
>
> **Versão:** 0.1 — consolidação das decisões narrativas e proposta de estrutura jogável.
>
> **Legenda:**
>
> - **[CÂNONE]:** confirmado pelo criador.
> - **[PROPOSTA]:** sugestão de design ainda não aprovada; inclui propostas visuais e de animação.
> - **[A DEFINIR]:** decisão em aberto.
> - **[SEGREDO]:** informação de bastidores que personagens ou jogadores podem desconhecer.

Consulte o [README](../README.md) para a referência geral da continuidade e as fichas de
[Lucy](../lucy.md) e [Nero](../nero.md) para os detalhes dos personagens. As propostas deste
documento não representam sistemas já implementados.

## Referências visuais de Little Garden

As imagens abaixo são turnarounds e estudos de sprites para orientar a produção visual do jogo. Elas
são referências de desenvolvimento, não arte final aprovada.

- [Turnaround de Lucy e Nero](assets/little-garden-turnaround-1.jpg): vistas, expressões, roupas e
  formas animais.
- [Sprites e perspectivas de gameplay](assets/little-garden-turnaround-2.jpg): referências para
  Topdown, Plataforma, ações, equipamentos e exploração.

---

## Sumário

Use os links abaixo para navegar entre a visão do jogo, seus sistemas propostos e as decisões
pendentes.

1. [Identidade e visão](#1-identidade-e-visão)
2. [Lugar na franquia e cronologia](#2-lugar-na-franquia-e-cronologia)
3. [Premissa e experiência pretendida](#3-premissa-e-experiência-pretendida)
4. [Universo e cenário](#4-universo-e-cenário)
5. [Personagens e elenco](#5-personagens-e-elenco)
6. [Estrutura narrativa da campanha](#6-estrutura-narrativa-da-campanha)
7. [Exame de afinidade da guilda](#7-exame-de-afinidade-da-guilda)
8. [Progressão de Lucy](#8-progressão-de-lucy)
9. [Nero e a cooperação](#9-nero-e-a-cooperação)
10. [Exploração, missões e encontros](#10-exploração-missões-e-encontros)
11. [Minigames e atividades da guilda](#11-minigames-e-atividades-da-guilda)
12. [Forja, materiais e equipamentos](#12-forja-materiais-e-equipamentos)
13. [Magia e treinamento](#13-magia-e-treinamento)
14. [Combate e desafios](#14-combate-e-desafios)
15. [Economia, recompensas e ritmo](#15-economia-recompensas-e-ritmo)
16. [Mundo, interface e acessibilidade](#16-mundo-interface-e-acessibilidade)
17. [Direção artística, áudio e animação](#17-direção-artística-áudio-e-animação)
18. [Estrutura técnica e dados](#18-estrutura-técnica-e-dados)
19. [Escopo e plano de produção](#19-escopo-e-plano-de-produção)
20. [Segredos, continuidade e limites do cânone](#20-segredos-continuidade-e-limites-do-cânone)
21. [Questões pendentes e critérios de aprovação](#21-questões-pendentes-e-critérios-de-aprovação)
22. [Resumo executivo](#resumo-executivo)

---

## 1. Identidade e visão

O quadro reúne a identidade do projeto, os elementos estabelecidos e as principais decisões ainda em
aberto.

| Campo                                               | Definição                                                                                                                             |
| --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| **Título**                                          | **Lucy & Nero — Little Garden**                                                                                                       |
| **Franquia**                                        | Lucy & Nero                                                                                                                           |
| **Posição comercial**                               | **Primeiro jogo a ser lançado** [CÂNONE]                                                                                              |
| **Posição cronológica**                             | Depois do encontro de Lucy e Nero; antes de _Entre Espadas e Garras_ [CÂNONE]                                                         |
| **Protagonistas**                                   | Lucy e Nero [CÂNONE]                                                                                                                  |
| **Cenário central**                                 | Vila de Lucy e seus arredores [CÂNONE]                                                                                                |
| **Tema central**                                    | Aprendizado, amizade, pequenas aventuras e desenvolvimento de habilidades                                                             |
| **Elementos confirmados**                           | Minigames, exploração, encontros aleatórios com inimigos, coleta de materiais, forja, treinamento e tarefas administrativas da guilda |
| **Grande marco narrativo**                          | Exame mágico de Lucy, por volta dos 12 anos [CÂNONE]                                                                                  |
| **Perspectivas de gameplay**                        | Topdown para exploração; Plataforma para combate, aulas e minigames [CÂNONE]                                                          |
| **Plataformas, engine e tecnologia**                | [A DEFINIR]                                                                                                                           |
| **Classificação indicativa, monetização e duração** | [A DEFINIR]                                                                                                                           |

### 1.1. Visão do projeto

**[CÂNONE]** _Little Garden_ apresenta Lucy como uma jovem aprendiz da Guilda dos Aventureiros,
acompanhada de Nero. Em vez de começar como uma heroína que já domina magia e forja, Lucy aprende a
partir de tarefas pequenas, prática artesanal, coleta, treinamentos e experiências cotidianas.

A campanha tem uma transformação importante: **antes do exame**, Lucy depende sobretudo de técnicas
aprendidas e materiais; **depois do exame**, passa a desenvolver conscientemente suas afinidades
mágicas com instrutores especializados. A forja e as aventuras continuam relevantes nas duas fases.

### 1.2. Princípios de design

Os princípios abaixo orientam a proposta de experiência a partir da formação de Lucy e de sua
parceria com Nero.

1. **Aprender fazendo:** novas capacidades devem surgir de experiências e treinamento, não apenas de
   exposição narrativa.
2. **A guilda é um lugar de trabalho:** missões e combate coexistem com registros, organização e
   responsabilidades administrativas.
3. **Pequenas aventuras importam:** o jogo não precisa antecipar a ameaça mundial da sequência.
4. **Nero é parceiro, não acessório:** sua inteligência animal e suas formas têm relevância
   narrativa e funcional.
5. **Mana não equivale a domínio:** a reserva gigantesca de Lucy não elimina a necessidade de
   aprender magia.
6. **O exame é uma virada, não o fim:** sua revelação abre novas possibilidades de gameplay.
7. **O mistério maior permanece:** a habilidade inata **Forjadora de Mundos** não é descoberta neste
   jogo.

---

## 2. Lugar na franquia e cronologia

A ordem dos acontecimentos distingue a posição narrativa de Little Garden de sua prioridade de
lançamento.

### 2.1. Os três projetos

Os três jogos ocupam períodos diferentes da trajetória dos protagonistas.

| Cronologia | Jogo                                          | Função narrativa                                                            |
| ---------- | --------------------------------------------- | --------------------------------------------------------------------------- |
| 1          | **As Crônicas de Nero** (ou _Contos do Nero_) | Aventuras solo de Nero, terminando no encontro com Lucy                     |
| 2          | **Lucy & Nero — Little Garden**               | Formação de Lucy, amizade, guilda, forja e despertar das afinidades         |
| 3          | **Lucy & Nero — Entre Espadas e Garras**      | Lucy e Nero enfrentam uma ameaça mundial; descoberta da Forjadora de Mundos |

**[CÂNONE]** _Little Garden_ é o primeiro lançamento, mesmo que _As Crônicas de Nero_ seja um
prelúdio cronológico.

### 2.2. Idades e eventos

Os marcos abaixo preservam a diferença de cinco anos entre Lucy e Nero.

| Evento                             |          Lucy |          Nero | Estado                                         |
| ---------------------------------- | ------------: | ------------: | ---------------------------------------------- |
| Nascimento de Lucy                 |             0 |             5 | [CÂNONE] Diferença etária de cinco anos        |
| Primeiro encontro                  |             7 |            12 | [CÂNONE] Encerramento de _As Crônicas de Nero_ |
| Início de _Little Garden_          |             9 |            14 | [CÂNONE] Início da campanha                    |
| Exame de afinidade                 |            12 |            17 | [CÂNONE] Acontecimento de _Little Garden_      |
| Encerramento de _Little Garden_    |            13 |            18 | [CÂNONE] Antes de Lucy completar 14 anos       |
| Início de _Entre Espadas e Garras_ | Depois dos 16 | Depois dos 21 | [CÂNONE] Aventura posterior                    |

**[CÂNONE]** _Little Garden_ começa quando Lucy tem 9 anos e termina aos 13, antes de ela completar
14 anos. Os anos 9, 10 e 11 ocupam aproximadamente a primeira metade da campanha, com passagem mais
rápida do tempo. Os anos 12 e 13 ocupam a segunda metade, pois concentram o exame, a descoberta
pública das afinidades, o treinamento mágico e mais elementos narrativos.

O encontro acontece quando Lucy tem 7 anos; _Little Garden_ começa dois anos depois. _Entre Espadas
e Garras_ acontece depois dos 16 anos de Lucy, com um intervalo posterior ao encerramento de _Little
Garden_.

---

## 3. Premissa e experiência pretendida

Esta seção relaciona a premissa narrativa à experiência desejada e ao ciclo de jogo proposto.

### 3.1. Sinopse interna

**[CÂNONE]** Lucy cresce como aprendiz da Guilda dos Aventureiros, explorando os arredores de sua
vila ao lado de Nero. Ela recolhe materiais, aprende técnicas de fabricação, participa de
treinamentos e ajuda a manter a guilda funcionando. Conforme progride, começa a aprender com Nero
uma forma de magia que ninguém reconhece como elemento: as sombras.

Em torno dos 12 anos, já na segunda metade da campanha, chega a hora do exame da guilda. O resultado
surpreende a todos: Lucy demonstra afinidade com **todos os elementos conhecidos**, além da
misteriosa magia das sombras. A descoberta transforma sua formação, abrindo caminho para instrutores
elementais e novas aplicações de magia na forja e nas aventuras.

**[SEGREDO]** Apesar de tudo, Lucy ainda não sabe que é a **Forjadora de Mundos**, e Nero não sabe
que é um **Neko Ryuu**.

### 3.2. Fantasia de jogador

**[PROPOSTA]** A sensação desejada é passar de uma aprendiz que precisa encontrar materiais e
executar tarefas simples para uma aventureira versátil, capaz de combinar fabricação, exploração,
magia e cooperação com Nero — sem deixar de pertencer à comunidade da vila.

### 3.3. Ciclo principal de jogo

**[PROPOSTA]** O fluxo abaixo propõe conectar tarefas, preparação, exploração e aprendizado em uma
sequência recorrente.

```text
Receber uma tarefa / descobrir uma oportunidade
              ↓
Preparar ferramentas e equipamentos
              ↓
Explorar, coletar, treinar ou executar a atividade
              ↓
Resolver um desafio / minigame / encontro
              ↓
Entregar, fabricar, registrar ou aprimorar
              ↓
Ganhar experiência prática e novas responsabilidades
              ↺
```

**[PROPOSTA]** Ciclos secundários: explorar → coletar → forjar; aceitar contrato → concluir →
registrar; treinar → dominar técnica → acessar novo desafio; observar Nero → experimentar sombra →
aprender uso novo.

---

## 4. Universo e cenário

A ambientação combina um mundo de magia ancestral com aventuras concentradas na vila e em seus
arredores.

### 4.1. Contexto histórico

**[CÂNONE]** O mundo já possui magia, monstros, mitologias e instituições estabelecidas há muito
tempo. A magia **não** surgiu recentemente. Neko Ryuu são criaturas mitológicas ancestrais; a guilda
é uma organização consolidada.

### 4.2. A vila

**[CÂNONE]** A vila de Lucy e seus arredores constituem o espaço central de _Little Garden_.

**[PROPOSTA]** Distribuir atividades entre um pequeno conjunto de lugares reutilizáveis, que mudam
de significado à medida que Lucy progride:

| Espaço                   | Uso sugerido                                       | Estado                                           |
| ------------------------ | -------------------------------------------------- | ------------------------------------------------ |
| Sede da guilda           | Missões, registros, exame, instrutores             | Guilda confirmada; organização espacial proposta |
| Oficina de forja         | Ferramentas, receitas, fabricação e aprimoramentos | Função confirmada; localização proposta          |
| Área de treinamento      | Prática de armas e magia                           | Treinamento confirmado; localização proposta     |
| Praça / comércio         | Personagens recorrentes e pedidos                  | [PROPOSTA]                                       |
| Floresta próxima         | Coleta, encontros e exploração                     | [PROPOSTA]                                       |
| Campos e trilhas         | Missões, deslocamento e descobertas                | [PROPOSTA]                                       |
| Ruínas / cavernas locais | Desafios mais complexos                            | [PROPOSTA]                                       |

**[A DEFINIR]** Nome da vila, mapa, biomas, clima, distâncias, NPCs e limites de exploração.

### 4.3. Guilda dos Aventureiros

**[CÂNONE]** Lucy é aprendiz; treina com membros da guilda e também realiza tarefas administrativas.
A guilda promove exames de afinidade mágica por volta dos 12 anos.

**[PROPOSTA]** A guilda funciona como eixo organizador: mural de pedidos, balcão administrativo,
registros, tutores, oficina associada e marcos de promoção. Não está confirmado que exista sistema
de patentes ou hierarquia específica.

---

## 5. Personagens e elenco

Lucy e Nero formam a dupla central, enquanto instrutores, familiares e demais personagens possuem
diferentes graus de definição.

### 5.1. Lucy

**[CÂNONE]** Humana, cinco anos mais nova que Nero. Aprende forja desde cedo, inicialmente sem
dominar magia. Possui uma quantidade de mana **igual à de Nero**, embora Nero seja um ser
constituído inteiramente de mana. Sua reserva extraordinária permite que o corpo regenere
ferimentos; isso **não é uma habilidade inata de cura**.

#### Trajetória neste jogo

A trajetória planejada de Lucy reúne os marcos de formação descritos abaixo.

- Aprendiz da guilda, envolvida em exploração e trabalho administrativo.
- Aprende técnicas de forja por coleta, ferramentas, prática e minigames.
- Desenvolve gradualmente o uso de sombras com Nero.
- Descobre no exame sua afinidade com fogo, água, eletricidade, vento e sombras.
- Passa a estudar os elementos com instrutores especializados.
- **Não descobre** que é a Forjadora de Mundos.

#### Aparência por período

**[PROPOSTA VISUAL]** Uma versão infantil/juvenil de Lucy deve ser criada especificamente para
_Little Garden_, preservando olhos verde-esmeralda, cabelos longos e escuros e uma identidade visual
que evolua para o traje preto, vermelho e dourado de _Entre Espadas e Garras_. Não copiar
integralmente o equipamento avançado da versão de 16 anos.

### 5.2. Nero

**[CÂNONE]** Companheiro de Lucy, cinco anos mais velho. Sua forma original é um **gato Bengal
melanístico**, preto com rosetas escuras e olhos verde-esmeralda. Não fala nem utiliza telepatia
convencional; expressa-se como animal, embora possua inteligência excepcional.

**[SEGREDO]** É um **Neko Ryuu** (Gato Dragão), criatura ancestral constituída inteiramente de mana,
ainda filhote e inconsciente de sua própria espécie. Sua habilidade inata individual é **Dragão das
Sombras**. Essa habilidade não é característica geral dos Neko Ryuu.

#### Formas e utilidades

As formas conhecidas de Nero oferecem vantagens distintas; sua disponibilidade durante a campanha
permanece em aberto.

| Forma      | Benefício                                                      | Regra de mana                                                               |
| ---------- | -------------------------------------------------------------- | --------------------------------------------------------------------------- |
| **Gato**   | Melhor agilidade, reação, expressividade e controle de sombras | Forma original                                                              |
| **Corvo**  | Voo, observação distante e visão excelente                     | Tamanho equivalente ao gato; não exige reserva adicional para ampliar corpo |
| **Cavalo** | Força, velocidade e transporte de pessoas                      | Exige reserva elevada para sustentar o corpo maior                          |

**[CÂNONE]** Trocar de forma não consome mana definitivamente: a reserva é comprometida enquanto
sustenta a forma e recuperada ao retornar à forma de gato. Nero assume animais que conheceu, com os
quais criou vínculos e cuja utilidade compreende. **[A DEFINIR]** Em que ponto de _Little Garden_
cada forma estará disponível ao jogador.

### 5.3. Instrutores e personagens secundários

**[CÂNONE]** Após o exame, Lucy terá instrutores para cada elemento conhecido; Nero é o instrutor
das sombras.

| Função                            | Identidade  | Situação          |
| --------------------------------- | ----------- | ----------------- |
| Instrutor de fogo                 | [A DEFINIR] | Função confirmada |
| Instrutor de água                 | [A DEFINIR] | Função confirmada |
| Instrutor de eletricidade         | [A DEFINIR] | Função confirmada |
| Instrutor de vento                | [A DEFINIR] | Função confirmada |
| Instrutor de sombras              | **Nero**    | [CÂNONE]          |
| Responsável pela formação de Lucy | [A DEFINIR] | [PROPOSTA]        |
| Responsável administrativo        | [A DEFINIR] | [PROPOSTA]        |
| Artesão/mentor de forja           | [A DEFINIR] | [PROPOSTA]        |
| Amigos, colegas e rivais          | [A DEFINIR] | [PROPOSTA]        |

### 5.4. Família de Lucy

**[CÂNONE]** O pai de Lucy, **Matthew**, realizou um sacrifício importante. **Somente esse
acontecimento** foi preservado da história original; suas circunstâncias ainda serão reescritas.
**Sarah** era o nome da mãe na versão antiga, mas sua caracterização na nova continuidade não está
confirmada. Não reutilizar automaticamente o antigo espírito, profecia, origem recente da magia ou
circunstâncias antigas do nascimento.

---

## 6. Estrutura narrativa da campanha

A campanha se organiza em torno da formação anterior ao exame e do aprendizado mágico que se segue a
ele.

### 6.1. Estrutura em duas grandes etapas

**[CÂNONE]** Há uma diferença clara entre a formação anterior e posterior ao exame da guilda. O
exame ocorre aproximadamente do meio do jogo em diante.

#### Etapa A — Formação artesanal e vida na guilda

**Foco confirmado:** anos 9, 10 e 11 de Lucy, com passagem mais rápida do tempo. A etapa concentra
coleta, minigames de forja, tarefas administrativas, pequenas aventuras, treinamentos e aprendizado
inicial das sombras.

**[PROPOSTA]** Dividir em capítulos de progressão:

1. **Primeiras responsabilidades:** apresentação da vila, da guilda, das ferramentas e da parceria
   com Nero.
2. **Aprendiz em atividade:** contratos simples, exploração e coleta, primeiras peças forjadas.
3. **Um mundo além da oficina:** tarefas mais exigentes, domínio de ferramentas e observação de
   poderes sombrios.
4. **Preparação para o exame:** treino, expectativas da comunidade e consolidação dos conhecimentos
   adquiridos.

#### Ponto de virada — Exame de afinidade

**[CÂNONE]** Lucy revela afinidade com todos os elementos conhecidos e com sombras, elemento até
então desconhecido. Isso se torna público. A habilidade Forjadora de Mundos **não** é detectada.

#### Etapa B — Formação mágica

**Foco confirmado:** anos 12 e 13 de Lucy, com mais espaço narrativo para instrução por elemento,
Nero como professor de sombras e continuidade do desenvolvimento de Lucy.

**[PROPOSTA]** Capítulos:

1. **O resultado impossível:** consequências imediatas do exame e apresentação dos instrutores.
2. **Quatro caminhos, uma aprendiz:** treinamentos elementais e novas aplicações na exploração.
3. **A quinta afinidade:** aprofundamento do ensino de sombras por Nero e novas possibilidades de
   cooperação.
4. **A forja evolui:** integração entre materiais, runas e propriedades elementais.
5. **Conclusão da formação inicial:** uma aventura local de encerramento que teste habilidades
   aprendidas, sem antecipar a ameaça mundial.

**[A DEFINIR]** Número real de capítulos, ritmo interno de cada ano, final, antagonistas locais e
quais saltos temporais representar diretamente. A divisão entre as duas metades orienta o ritmo, mas
não fixa a duração de cada capítulo.

### 6.2. Tipo de história

**[CÂNONE]** Pequenas aventuras próximas à vila, com minigames e inimigos que aparecem ao acaso.

**[PROPOSTA]** Alternar histórias cotidianas, pedidos de moradores, desafios de guilda, treinamento
e episódios mais marcantes. Evitar transformar todo pedido em uma crise épica.

### 6.3. Marcos narrativos obrigatórios

A lista abaixo permite conferir a presença dos marcos de continuidade previstos para a campanha.

- [ ] Mostrar Lucy como aprendiz, não como aventureira plenamente formada.
- [ ] Estabelecer a guilda como instituição antiga e funcional.
- [ ] Apresentar coleta e forja antes da magia elemental controlada.
- [ ] Mostrar Nero como parceiro inteligente, não falante.
- [ ] Introduzir o aprendizado de sombras **antes** do exame.
- [ ] Estabelecer que a mana de Lucy já é reconhecida como extraordinária.
- [ ] Realizar o exame por volta dos 12 anos.
- [ ] Revelar publicamente as afinidades de Lucy.
- [ ] Introduzir instrutores dos quatro elementos conhecidos.
- [ ] Manter Nero como único instrutor de sombras.
- [ ] Encerrar sem revelar a habilidade Forjadora de Mundos.

---

## 7. Exame de afinidade da guilda

O exame é o marco público das afinidades de Lucy e altera sua formação sem revelar habilidades
inatas.

### 7.1. Função no universo

**[CÂNONE]** É um exame tradicional realizado normalmente em torno dos 12 anos para descobrir as
**afinidades mágicas** dos jovens.

**Regra absoluta:** **não detecta habilidades inatas**.

### 7.2. Situação de Lucy antes do exame

Os pontos abaixo descrevem o que já se manifesta na vida de Lucy antes da avaliação da guilda.

- Sua reserva colossal de mana já é conhecida.
- Sua capacidade de regenerar ferimentos já é conhecida.
- Ela ainda não domina conscientemente os elementos convencionais.
- Já começou a aprender sombras através de Nero.
- Nem Lucy nem Nero entendem plenamente que compartilham poderes.

### 7.3. Resultado

O resultado revela compatibilidade com os elementos conhecidos e torna pública a afinidade com
sombras.

| Afinidade    | Situação anterior                     | Resultado                                                             |
| ------------ | ------------------------------------- | --------------------------------------------------------------------- |
| Fogo         | Elemento conhecido                    | Lucy é compatível                                                     |
| Água         | Elemento conhecido                    | Lucy é compatível                                                     |
| Eletricidade | Elemento conhecido                    | Lucy é compatível                                                     |
| Vento        | Elemento conhecido                    | Lucy é compatível                                                     |
| Sombras      | Elemento não reconhecido publicamente | Lucy manifesta a afinidade; a existência do elemento torna-se pública |

**[CÂNONE]** A afinidade com todos os elementos conhecidos é algo inconcebível e nunca antes
registrado.

### 7.4. Consequências

**[CÂNONE]** Lucy passa a estudar com instrutores de cada elemento. Nero ensina sombras, que apenas
os dois controlam nesse estágio da história.

**[PROPOSTA]** O exame pode ser uma missão narrativa especial com preparação, observação de outros
jovens, apresentação do procedimento, resultado e repercussão na guilda. Não definir ainda o
aparelho, ritual, pontuação, autoridades presentes ou reação específica dos NPCs.

### 7.5. O que não deve acontecer

As restrições abaixo preservam a função do exame e as distinções do sistema mágico.

- O exame **não** anuncia Lucy como Forjadora de Mundos.
- O exame **não** identifica o poder inato de Nero.
- O exame **não** revela que Nero é Neko Ryuu.
- A regeneração de Lucy **não** deve ser apresentada como magia inata de cura.
- A revelação das sombras **não** implica que magia e monstros surgiram recentemente.

---

## 8. Progressão de Lucy

A progressão articula competências aprendidas sem confundir reserva de mana com domínio técnico.

### 8.1. Eixos confirmados

A formação de Lucy envolve os cinco eixos descritos a seguir.

1. **Forja:** habilidade construída por prática, materiais e minigames.
2. **Formação de aventureira:** treinamento e pequenas missões.
3. **Administração da guilda:** tarefas organizacionais reais.
4. **Sombras:** aprendizado progressivo com Nero, iniciado antes do exame.
5. **Elementos:** treinamento estruturado após o exame.

### 8.2. Modelo de progressão sugerido

**[PROPOSTA]** Em vez de um nível único, usar progressões de competência separadas:

| Trilha    | Antes do exame                        | Depois do exame                                  |
| --------- | ------------------------------------- | ------------------------------------------------ |
| Forja     | Ferramentas, materiais, peças simples | Runas, propriedades elementais, combinações      |
| Aventura  | Exploração local, contratos simples   | Desafios que exigem novas técnicas               |
| Guilda    | Registro e organização básicos        | Pedidos e responsabilidades mais complexos       |
| Sombras   | Observação, primeiros usos            | Técnicas mais consistentes e cooperação          |
| Elementos | Ainda não dominados                   | Fogo, água, eletricidade e vento com instrutores |

**[PROPOSTA]** Cada trilha pode desbloquear atividades por marcos de domínio, receitas aprendidas,
conclusão de treinamentos ou autorização da guilda. Não fixar níveis numéricos antes de testar o
ritmo.

### 8.3. Equilíbrio narrativo

Lucy **não** precisa começar fraca em quantidade de mana; ela começa **inexperiente no controle**.
Isso permite que sua enorme reserva exista desde o início sem eliminar o desafio de aprender
técnicas.

**[A DEFINIR]** Quais habilidades de combate Lucy conhece antes do exame, quais aprende depois e
quando passa a utilizar katana, arco e escudo com segurança.

---

## 9. Nero e a cooperação

Nero participa como companheiro e instrutor; as formas de controle e interação com o jogador ainda
precisam ser definidas.

### 9.1. Papel central

**[CÂNONE]** Nero é companheiro e instrutor de sombras. Seu vínculo com Lucy é recíproco, construído
pela convivência, e permite compartilhamento de poderes sem que ambos compreendam inicialmente o
mecanismo.

### 9.2. Cooperação no gameplay

**[PROPOSTA]** Possíveis interações:

- **Gato:** investigar espaços pequenos, perceber sinais e demonstrar pistas por comportamento.
- **Corvo:** observar regiões elevadas, reconhecer caminhos e localizar pontos de interesse.
- **Cavalo:** transportar Lucy por áreas maiores, quando a forma estiver disponível.
- **Sombra:** ocultação, acesso ao inventário e demonstrações de técnicas.

**[A DEFINIR]** Nero será controlável diretamente, comandado por ações contextuais ou operará com IA
autônoma? Quais formas estarão disponíveis em cada capítulo?

### 9.3. Comunicação

**[CÂNONE]** Nero não fala nem transmite conversas por telepatia. Sua inteligência excepcional se
expressa por ações, sons e linguagem corporal animal.

**[PROPOSTA]** Usar animações de orelhas, cauda, postura, olhar, vocalizações e pequenas ações
contextuais como feedback para o jogador. Evitar legendas que atribuam fala literal a Nero como se
fossem diálogos canônicos.

### 9.4. Compartilhamento mágico

**[CÂNONE]** Lucy aprende sombras por causa da relação com Nero; o fenômeno de compartilhamento é
mútuo.

**[A DEFINIR]** Quais manifestações elementais Nero poderá usar neste jogo e em que momento Lucy
desenvolverá equipamentos que ampliem essas capacidades. Não assumir transferência irrestrita de
todos os poderes.

### 9.5. Inventário sombrio

**[CÂNONE]** Lucy pode guardar materiais, ferramentas, armas e objetos físicos na própria sombra,
funcionando como inventário de capacidade descrita como infinita. Nero pode acessá-lo.

**[PROPOSTA]** A interface pode organizar categorias e filtros para facilitar o uso, sem inventar um
limite de capacidade narrativo. **[A DEFINIR]** Quando o jogador desbloqueia o inventário e quais
restrições de interface/uso são adequadas.

---

## 10. Exploração, missões e encontros

As aventuras locais combinam coleta, tarefas e encontros, com modelos de exploração ainda propostos.

### 10.1. Exploração

**[CÂNONE]** Aventura nos arredores da vila, com coleta e encontros ocasionais com inimigos.

**[PROPOSTA]** Exploração baseada em áreas interligadas, cada uma com recursos, pequenas histórias e
mudanças após marcos de progressão. A topologia exata não está definida; não presumir mundo aberto.

### 10.2. Categorias de tarefas

A tabela apresenta exemplos propostos de atividades e identifica sua relação com os conceitos
confirmados.

| Categoria     | Exemplo de atividade                            | Status                                       |
| ------------- | ----------------------------------------------- | -------------------------------------------- |
| Coleta        | Encontrar recursos para fabricar uma peça       | [PROPOSTA] baseada na coleta confirmada      |
| Entrega       | Levar material ou pedido a um morador           | [PROPOSTA]                                   |
| Administração | Classificar solicitações ou conferir registros  | [PROPOSTA] baseada no trabalho confirmado    |
| Treinamento   | Praticar técnica com um membro da guilda        | [PROPOSTA] baseada no treinamento confirmado |
| Exploração    | Investigar trilha, bosque ou ponto de interesse | [PROPOSTA]                                   |
| Proteção      | Lidar com encontro perigoso próximo à vila      | [PROPOSTA]                                   |
| Artesanato    | Fabricar equipamento sob encomenda              | [PROPOSTA]                                   |

### 10.3. Encontros aleatórios

**[CÂNONE]** Inimigos podem aparecer ao acaso durante as aventuras.

**[PROPOSTA]** Definir tabelas de encontro por região e fase da campanha, evitando interrupções
excessivas. A frequência deve permitir exploração tranquila e treinamento sem tornar o combate
obrigatório a todo instante.

**[A DEFINIR]** Tipos de inimigos, comportamento, recompensas, raridade e forma de transição para o
combate.

### 10.4. Rejogabilidade

**[PROPOSTA]** Pedidos repetíveis, variações de minigames, materiais em locais alternativos e
desafios opcionais. Repetição deve servir ao aprendizado, não exigir trabalho excessivo para acessar
a história.

---

## 11. Minigames e atividades da guilda

Os minigames traduzem a formação de Lucy em atividades práticas; o catálogo e as mecânicas ainda
precisam ser validados.

### 11.1. Papel dos minigames

**[CÂNONE]** Os minigames são centrais para o desenvolvimento da forja de Lucy e para o cotidiano do
jogo.

**[PROPOSTA]** Cada minigame deve ensinar uma competência, oferecer feedback claro e evoluir em
dificuldade com o treinamento.

### 11.2. Minigames sugeridos

As atividades abaixo são sugestões para desenvolver fabricação, administração e treinamento.

| Atividade                   | Mecânica sugerida                                      | Progressão sugerida                           |
| --------------------------- | ------------------------------------------------------ | --------------------------------------------- |
| **Preparação de materiais** | Separar, medir ou combinar componentes                 | Mais tipos de material e exigências           |
| **Forja**                   | Controlar etapas de aquecimento, moldagem e acabamento | Peças mais complexas e técnicas novas         |
| **Gravação rúnica**         | Aplicar padrões ou sequências                          | Disponível após aprendizado mágico apropriado |
| **Registro de contratos**   | Organizar pedidos e identificar informações            | Mais campos e prioridades                     |
| **Inventário da guilda**    | Conferir entradas, saídas e entregas                   | Pedidos simultâneos e exceções                |
| **Treino de arco**          | Precisão e tempo de disparo                            | Alvos com padrões variados                    |
| **Treino de defesa**        | Reconhecer e responder a ataques                       | Combinações mais elaboradas                   |
| **Treino elemental**        | Reproduzir técnicas com feedback do instrutor          | Controle progressivo de cada elemento         |
| **Treino de sombras**       | Observar demonstrações de Nero e reproduzir usos       | Aplicações gradualmente mais complexas        |

**Nota:** nenhum minigame específico da tabela está confirmado como implementação definitiva; são
propostas para materializar as atividades já estabelecidas.

### 11.3. Regras de boa experiência

**[PROPOSTA]** As orientações abaixo propõem critérios para tornar as atividades compreensíveis,
acessíveis e relevantes para o aprendizado.

- Explicar objetivos antes de iniciar.
- Permitir repetição sem punição narrativa excessiva.
- Distinguir falha de treinamento de falha definitiva de missão.
- Recompensar melhora real de execução.
- Evitar depender exclusivamente de reflexos rápidos.
- Oferecer alternativas de acessibilidade para ações de precisão/tempo.
- Não transformar tarefas administrativas em preenchimento burocrático sem significado.

---

## 12. Forja, materiais e equipamentos

A forja conecta coleta, prática e equipamentos, expandindo suas possibilidades conforme Lucy aprende
magia.

### 12.1. Identidade da forja

**[CÂNONE]** Lucy começa aprendendo fabricação **sem dominar magia**. Ela precisa coletar materiais
e praticar através de minigames. A forja é uma habilidade aprendida e **não é** a manifestação
automática da habilidade inata Forjadora de Mundos.

### 12.2. Fluxo de fabricação

**[PROPOSTA]** O fluxo sugerido organiza o caminho entre a necessidade de uma peça e seu uso após a
fabricação.

```text
Descobrir pedido ou receita
          ↓
Conseguir materiais
          ↓
Preparar ferramentas e componentes
          ↓
Executar minigame de fabricação
          ↓
Avaliar resultado e concluir peça
          ↓
Equipar / entregar / guardar / aprimorar
```

### 12.3. Progressão de receitas

**[PROPOSTA]** As etapas abaixo propõem uma evolução da fabricação comum para aplicações mágicas e
equipamentos de Nero.

| Etapa               | Tipo de produção                              | Requisitos                        |
| ------------------- | --------------------------------------------- | --------------------------------- |
| Inicial             | Ferramentas e peças comuns                    | Materiais, ferramentas e técnica  |
| Intermediária       | Equipamentos de melhor acabamento             | Receitas e domínio de forja       |
| Pós-exame           | Peças com propriedades mágicas                | Conhecimento elemental e rúnico   |
| Avançada neste jogo | Combinações de propriedades e itens para Nero | Treinamento, materiais e receitas |

**[A DEFINIR]** Tipos exatos de armas, raridade, durabilidade, atributos e quais receitas estarão
presentes.

### 12.4. Elementos e runas

**[CÂNONE]** Lucy desenvolve equipamentos rúnicos e pode incorporar propriedades elementais à forja.

| Elemento     | Cor de referência | Aplicação ilustrativa — [PROPOSTA]      |
| ------------ | ----------------- | --------------------------------------- |
| Fogo         | Vermelho          | Efeito de calor                         |
| Água         | Azul              | Efeito fluido ou aquático               |
| Eletricidade | Amarelo           | Descarga elétrica                       |
| Vento        | Verde             | Impulso ou corrente de ar               |
| Sombras      | Escuro            | Interação com ocultação e armazenamento |

**[A DEFINIR]** Regras de combinação, custos, limites e efeitos concretos no gameplay.

### 12.5. Equipamentos para Nero

**[CÂNONE]** Lucy fabrica equipamentos rúnicos para que Nero também utilize propriedades elementais.
Identidade cromática de seus artefatos: **preto, dourado e verde-esmeralda**.

**[PROPOSTA VISUAL]** Garras e proteção felina, talões e penas encantadas para corvo, cascos e
arreios para cavalo. **[A DEFINIR]** Se são itens separados, se adaptam automaticamente e quando são
introduzidos em _Little Garden_.

---

## 13. Magia e treinamento

O treinamento diferencia afinidade, quantidade de mana e domínio efetivo das técnicas.

### 13.1. Princípio fundamental

**[CÂNONE]** Lucy possui mana colossal antes de saber controlar magia. O aprendizado não deve ser
substituído pela quantidade de energia disponível.

### 13.2. Antes do exame

Antes da avaliação da guilda, Lucy apresenta as capacidades e limitações abaixo.

- **Sombras:** aprendizado inicial com Nero [CÂNONE].
- **Fogo, água, eletricidade, vento:** não são ainda dominados conscientemente por Lucy [CÂNONE].
- **Regeneração:** consequência natural da quantidade de mana, já conhecida [CÂNONE].

### 13.3. Depois do exame

**[CÂNONE]** Lucy recebe instrução de cada elemento com especialistas. Nero ensina sombras.

**[PROPOSTA]** Cada disciplina pode ter uma sequência de demonstração → exercício → aplicação na
exploração → aplicação na forja → desafio de domínio.

### 13.4. Progressão sem contradição

Os cuidados abaixo mantêm o aprendizado coerente com as regras mágicas da franquia.

- Não tratar sombras como magia recém-criada: o **reconhecimento público** do elemento é novo, não
  necessariamente sua existência.
- Não tratar Lucy como capaz de lançar qualquer magia apenas por possuir afinidade.
- Não apresentar a Forjadora de Mundos como talento descoberto no exame.
- Não explicar a reserva de mana de Lucy com teorias ainda não confirmadas.
- Não pressupor que Nero tenha afinidade elemental própria com fogo, água, eletricidade e vento; seu
  uso desses efeitos pode depender dos equipamentos e do compartilhamento ainda em definição.

---

## 14. Combate e desafios

O combate integra a formação da aprendiz, enquanto outros desafios exploram fabricação,
administração e cooperação.

### 14.1. Papel do combate

**[CÂNONE]** Lucy treina com aventureiros e enfrenta inimigos encontrados ao acaso nas pequenas
aventuras.

**[PROPOSTA]** Combate acessível inicialmente, com complexidade crescente conforme a formação de
Lucy. O foco é desenvolver habilidade e cooperação, não começar com batalhas épicas.

### 14.2. Equipamentos de referência

**[CÂNONE NA FRANQUIA]** Lucy utiliza katana, arco e escudo na fase mais avançada de sua história.
**[A DEFINIR]** Em que momento cada arma é adquirida ou treinada em _Little Garden_.

**[PROPOSTA]**

- Katana: ataques de proximidade e técnica.
- Arco: precisão e distância.
- Escudo: defesa e leitura de ataques.
- Nero: reconhecimento, distração e apoio contextual, respeitando a forma atual.

### 14.3. Desafios além do combate

**[PROPOSTA]** Obstáculos de exploração, coleta, treinamento, fabricação e administração devem ser
tão relevantes quanto confrontos.

### 14.4. Derrota e recuperação

**[A DEFINIR]** Condições de derrota, retorno à guilda, perda de recursos, penalidades e como
representar a regeneração de Lucy sem anular o desafio. A regeneração não implica invulnerabilidade.

---

## 15. Economia, recompensas e ritmo

Recursos e recompensas devem sustentar a proposta de aprendizado, com economia e balanceamento ainda
em aberto.

### 15.1. Recursos

**[CÂNONE]** Coleta de materiais é necessária à forja.

**[PROPOSTA]** Organizar recursos por origem e uso (minerais, madeira, fibras, componentes mágicos
etc.). Nenhuma lista específica de materiais está aprovada.

### 15.2. Recompensas

**[PROPOSTA]** Priorizar recompensas que reforcem a formação:

- Novas receitas.
- Ferramentas melhores.
- Acesso a treinamentos.
- Autorização para missões mais complexas.
- Materiais raros.
- Novas interações com Nero.
- Conhecimento e técnicas mágicas.

**[A DEFINIR]** Moeda, preços, sistema de vendas, patentes, XP e balanceamento.

### 15.3. Ritmo de campanha

**[PROPOSTA]** Alternar aventura, minigame, conversa e progressão. O exame deve ser um ponto de
virada marcante, mas a segunda parte não deve abandonar as atividades artesanais e administrativas
que definem o jogo.

---

## 16. Mundo, interface e acessibilidade

Esta seção reúne decisões pendentes e propostas para navegação, apresentação das informações e
acesso às atividades.

### 16.1. Estrutura de mapa

**[CÂNONE]** O jogo combina duas perspectivas em uma mesma experiência:

- **Topdown:** visão principal para explorar a vila, regiões, missões, coleta, encontros e interação
  com personagens e objetos.
- **Plataforma:** visão lateral para combate detalhado, aulas de esgrima e magia, forja e outros
  minigames que dependem de movimento, precisão ou animações específicas.

**[PROPOSTA]** A transição ocorre quando Lucy inicia uma atividade compatível com a visão lateral.
Ao concluir, o jogo retorna ao mapa Topdown com os resultados obtidos. A câmera, a escala, o
carregamento de áreas, o fast travel, o ciclo de dia e noite e a navegação ainda precisam ser
definidos para cada perspectiva.

### 16.2. Regras de interação entre perspectivas

As duas visões devem compartilhar personagens, progresso, inventário e consequências narrativas.

- NPCs podem ser encontrados e receber pedidos no Topdown, e participar de cenas ou atividades em
  Plataforma.
- A exploração Topdown deve levar diretamente às atividades laterais, sem tratá-las como telas
  desconectadas.
- Combate e minigames em Plataforma devem devolver recompensas, ferimentos, materiais ou
  desbloqueios ao estado da exploração.
- O jogador deve reconhecer Lucy e Nero nas duas visões por silhueta, paleta e animações coerentes.
- As formas de Nero podem ter funções distintas em cada perspectiva, respeitando as regras de sua
  metamorfose e as formas disponíveis naquele momento.

### 16.3. Atividades em Plataforma

As atividades abaixo são a primeira proposta de escopo para a visão lateral. Cada uma ainda precisa
de protótipo e critérios de aprovação próprios.

| Atividade            | Função na campanha                                                             |
| -------------------- | ------------------------------------------------------------------------------ |
| Combate              | Encontros com movimentação, ataques, defesa e cooperação com Nero.             |
| Forja                | Minigames de preparação, fabricação, gravação rúnica e acabamento.             |
| Aulas de esgrima     | Treino de movimentação, armas, esquiva e defesa.                               |
| Aulas de magia       | Exercícios de controle dos elementos após os desbloqueios narrativos.          |
| Atividades da guilda | Tarefas administrativas ou interações que se beneficiem de animações e timing. |

**[PROPOSTA]** Priorizar uma vila reconhecível, com pontos de interesse persistentes e regiões
próximas reutilizadas com novas tarefas e desafios.

### 16.4. Interfaces necessárias

**[PROPOSTA]** A lista abaixo propõe interfaces para organizar as atividades e apresentar a
progressão ao jogador.

- Diário de tarefas e contratos.
- Inventário sombrio com filtros.
- Menu de materiais e receitas.
- Tela de fabricação/minigames.
- Registro de treinamentos e técnicas.
- Mapa da vila e arredores.
- Tela de progressão por competências.
- Registro de afinidades após o exame.
- Indicação contextual das ações de Nero.

### 16.5. Acessibilidade

**[PROPOSTA]** Remapeamento de controles, legendas, escala de texto, contraste, ajustes de
dificuldade dos minigames, assistência para ações de tempo/precisão e opção de repetir tutoriais. As
necessidades exatas dependem das plataformas escolhidas.

---

## 17. Direção artística, áudio e animação

A direção audiovisual parte das referências da franquia e propõe adaptações à fase de aprendizado
dos personagens.

### 17.1. Estilo visual

**[CÂNONE DE REFERÊNCIA]** Estética **anime/cartoon shounen 2D**, contornos limpos, cel shading e
silhuetas reconhecíveis. Evitar semi-realismo, estética seinen ou wuxia que se afaste das
referências dos personagens.

### 17.2. Lucy em Little Garden

**[PROPOSTA VISUAL]** Criar versões da personagem por etapa de idade/treinamento. A roupa deve
evoluir junto com a progressão: ferramentas e roupas simples antes da magia, detalhes rúnicos e
equipamentos especializados posteriormente. Não usar automaticamente o visual de 16 anos em cenas da
infância.

### 17.3. Nero

**[CÂNONE VISUAL]** Gato Bengal melanístico preto, rosetas sutis e olhos verde-esmeralda; formas de
corvo e cavalo preservam identidade cromática. Nero nunca deve parecer cachorro/lobo.

**[PROPOSTA DE ANIMAÇÃO]** Transformação com transição por **meia-sombra**, sombra completa e
reconstrução da forma animal. O design exato do estágio intermediário ainda precisa ser aprovado.
Manter anatomia correta, sem membros, cabeças ou caudas extras.

### 17.4. Efeitos mágicos

A tabela reúne as cores elementais de referência e a orientação visual geral sugerida para sombras.

| Elemento     | Identidade visual                                     |
| ------------ | ----------------------------------------------------- |
| Fogo         | Vermelho                                              |
| Água         | Azul                                                  |
| Eletricidade | Amarelo                                               |
| Vento        | Verde                                                 |
| Sombras      | Silhuetas e efeitos escuros, preservando legibilidade |

**[PROPOSTA]** A evolução visual da magia deve acompanhar o aprendizado: efeitos discretos e
imprecisos nas primeiras experiências; efeitos mais claros e controlados após treinamento.

### 17.5. Áudio

**[A DEFINIR]** Identidade musical, instrumentação, efeitos de guilda/oficina, sons dos elementos e
temas dos personagens.

**[CÂNONE]** Nero comunica-se por sons animais e comportamento, não por fala humana ou telepatia
convencional.

---

## 18. Estrutura técnica e dados

> Esta seção apresenta uma **proposta de arquitetura de produção**, não uma decisão confirmada sobre
> a engine ou implementação de _Little Garden_.

### 18.1. Sistemas de alto nível — [PROPOSTA]

A divisão abaixo propõe responsabilidades para uma implementação futura, sem fixar uma arquitetura
aprovada.

| Sistema      | Responsabilidade                                  |
| ------------ | ------------------------------------------------- |
| Progressão   | Técnicas, receitas, marcos e desbloqueios         |
| Missões      | Contratos, objetivos, estados e recompensas       |
| Guilda       | Registros, tarefas administrativas e treinamentos |
| Inventário   | Materiais, ferramentas, equipamentos e sombra     |
| Forja        | Receitas, requisitos, minigames e resultados      |
| Magia        | Afinidades, técnicas, treinamento e efeitos       |
| Nero         | Formas, comportamentos, habilidades e cooperação  |
| Encontros    | Aparição de inimigos por região e condições       |
| Mundo        | Áreas, recursos, eventos e exploração             |
| Persistência | Progresso, itens, missões e estado do mundo       |
| Interface    | HUD, menus, diálogos e feedback                   |

### 18.2. Dados orientados a conteúdo — [PROPOSTA]

Definir recursos estruturados para `Character`, `Ability`, `Element`, `Item`, `Recipe`, `Material`,
`Quest`, `Minigame`, `Training`, `EncounterTable`, `Region` e `StoryFlag`.

Exemplos de flags narrativas:

```text
met_nero = true
shadow_training_started = false
guild_exam_completed = false
all_known_affinities_revealed = false
shadow_affinity_public = false
elemental_training_unlocked = false
world_forger_discovered = false  # permanece false neste jogo
```

**Atenção:** valores e nomes são ilustrativos; não representam código de produção.

### 18.3. Persistência — [PROPOSTA]

Salvar pelo menos:

- Capítulo/etapa narrativa.
- Missões e registros administrativos.
- Materiais e equipamentos.
- Receitas aprendidas.
- Treinamentos concluídos.
- Estado de disponibilidade das formas de Nero.
- Técnicas de sombra aprendidas.
- Afinidades reveladas no exame.
- Estado de regiões e eventos importantes.

### 18.4. Integração futura com a franquia — [PROPOSTA]

Documentar quais informações são úteis para continuidade em _Entre Espadas e Garras_ (receitas,
personagens conhecidos, marcos da guilda), **sem assumir** que haverá importação direta de saves
entre jogos.

---

## 19. Escopo e plano de produção

Os protótipos e prioridades sugeridos procuram validar o ciclo central antes de expandir a produção.

### 19.1. Vertical slice sugerido

**[PROPOSTA]** Um protótipo curto capaz de provar o ciclo central:

1. Lucy recebe uma tarefa na guilda.
2. Explora uma área próxima.
3. Coleta materiais.
4. Encontra um desafio simples.
5. Retorna à oficina.
6. Executa um minigame de forja.
7. Entrega o resultado e recebe progresso.
8. Interage com Nero em uma ação contextual.

**Critério de sucesso:** esse ciclo deve ser divertido mesmo sem a magia elemental pós-exame.

### 19.2. Segundo protótipo sugerido

**[PROPOSTA]** Demonstrar a virada do exame: cena de revelação, atualização das afinidades, primeiro
treinamento elemental e primeiro uso mágico na forja.

### 19.3. Priorização

A tabela organiza prioridades sugeridas e distingue a confirmação conceitual do estado de
implementação.

| Prioridade | Entrega                                               | Estado                                        |
| ---------- | ----------------------------------------------------- | --------------------------------------------- |
| Essencial  | Vila, guilda, Lucy, Nero, exploração e tarefas        | Conceitos confirmados; implementação pendente |
| Essencial  | Coleta, forja e minigames                             | Conceitos confirmados; regras pendentes       |
| Essencial  | Exame e progressão pós-exame                          | Marco narrativo confirmado                    |
| Essencial  | Treinamento elemental e sombras                       | Conceitos confirmados                         |
| A validar  | Combate detalhado e frequência de encontros           | [A DEFINIR]                                   |
| A validar  | Controle direto de Nero                               | [A DEFINIR]                                   |
| A validar  | Economia, comércio e patentes                         | [A DEFINIR]                                   |
| Opcional   | Atividades adicionais, colecionáveis, desafios extras | [PROPOSTA]                                    |

### 19.4. Riscos de escopo

**[PROPOSTA]** Principais riscos: excesso de minigames diferentes, muitos elementos com sistemas
independentes, mundo grande demais, NPCs sem função clara e desenvolvimento simultâneo de todas as
formas de Nero. Mitigação: validar primeiro o ciclo da guilda e forja; depois testar a virada
mágica.

---

## 20. Segredos, continuidade e limites do cânone

Esta seção separa informações apresentáveis em Little Garden dos segredos e limites que orientam a
continuidade da franquia.

### 20.1. O que o jogador pode descobrir em Little Garden

As informações abaixo podem ser apresentadas ao longo da formação de Lucy e do exame.

- **[CÂNONE]** Lucy possui uma quantidade extraordinária de mana.
- **[CÂNONE]** Sua regeneração decorre dessa reserva.
- **[CÂNONE]** Lucy tem afinidade com fogo, água, eletricidade, vento e sombras.
- **[CÂNONE]** O resultado é inédito e inconcebível para o conhecimento da guilda.
- **[CÂNONE]** A magia das sombras se torna publicamente conhecida através dela.
- **[CÂNONE]** Nero ensina sombras a Lucy.

### 20.2. Segredos de bastidores

Os tópicos a seguir orientam a escrita interna e não implicam que todas as informações sejam
reveladas neste jogo.

#### Lucy é a Forjadora de Mundos

**[SEGREDO / CÂNONE]** Lucy possui essa habilidade inata, mas **não a descobre em Little Garden**.
Sua revelação pertence a _Entre Espadas e Garras_. Não sugerir que o exame seja capaz de detectá-la.

#### Nero é um Neko Ryuu

**[SEGREDO / CÂNONE]** Nero é um Gato Dragão, espécie ancestral de mana, e ainda é filhote. Ele
próprio desconhece sua natureza. Sua futura forma dracônica virá com a maturação natural, ao longo
de décadas e séculos.

#### Nero é o Dragão das Sombras

**[SEGREDO / CÂNONE]** A magia das sombras e a metamorfose em animais são poderes individuais de
Nero, não características de todos os Neko Ryuu.

#### O vínculo é recíproco

**[SEGREDO / CÂNONE]** Lucy e Nero compartilham poderes sem compreender o fenômeno. O mecanismo e a
extensão exata ainda não foram definidos.

#### Origem da mana de Lucy

**[SEGREDO / A DEFINIR]** Não foi explicado por que uma humana possui tanta mana quanto um Neko
Ryuu. Não atribuir essa condição a Matthew, a um espírito ou à habilidade Forjadora de Mundos sem
nova decisão.

#### Sacrifício de Matthew

**[CÂNONE PARCIAL]** Apenas o sacrifício do pai de Lucy foi preservado da narrativa antiga. As
circunstâncias serão reescritas. A história anterior sobre surgimento recente de magia/monstros,
espírito e profecia foi descontinuada.

### 20.3. Regras de continuidade

As regras abaixo resumem os pontos que devem permanecer consistentes durante o desenvolvimento.

1. Nero é **cinco anos mais velho** que Lucy.
2. Eles se conhecem quando Lucy tem **7** e Nero **12** anos.
3. Lucy tem **16** e Nero **21** em _Entre Espadas e Garras_.
4. O exame ocorre por volta dos **12 anos de Lucy**.
5. O exame identifica **afinidades**, nunca **habilidades inatas**.
6. A reserva de mana de Lucy equivale à de Nero.
7. A regeneração de Lucy decorre da reserva de mana.
8. Lucy aprende forja **antes** de dominar magia elemental.
9. Lucy começa a aprender sombras **antes** do exame.
10. A existência pública da magia das sombras é revelada no exame.
11. Nero é o instrutor de sombras de Lucy.
12. Nero **não fala** nem utiliza telepatia convencional.
13. Nero possui formas de **gato, corvo e cavalo**, não de cachorro/lobo.
14. As transformações de Nero não gastam mana definitivamente, mas exigem reserva para sustentar
    corpos maiores.
15. Nero não sabe que é Neko Ryuu.
16. A habilidade Forjadora de Mundos não é revelada em _Little Garden_.
17. A magia e os monstros são antigos; a guilda já é estabelecida.
18. A ameaça mundial pertence ao conceito de _Entre Espadas e Garras_, não precisa ser antecipada
    como conflito central de _Little Garden_.

---

## 21. Questões pendentes e critérios de aprovação

As listas registram decisões ainda necessárias e propõem critérios para avaliar a consolidação da
pré-produção.

### 21.1. Narrativa

Os aspectos narrativos abaixo ainda precisam de definição e aprovação.

- [ ] Distribuição exata dos capítulos entre os anos 9–11 e 12–13 de _Little Garden_.
- [ ] Como Lucy entra para a guilda.
- [ ] Relação de Lucy com a mãe/família na nova versão.
- [ ] Como o sacrifício de Matthew afeta a infância.
- [ ] Nome da vila e da guilda local.
- [ ] Personagens recorrentes e seus papéis.
- [ ] Estrutura definitiva dos capítulos.
- [ ] Evento de encerramento do jogo.
- [ ] Repercussão social e institucional do exame.

### 21.2. Gameplay

As decisões abaixo determinam o funcionamento e o escopo dos sistemas jogáveis.

- [ ] Gênero mecânico definitivo e perspectiva de câmera.
- [ ] Controle de Lucy e Nero.
- [ ] Sistema de combate.
- [ ] Lista final de minigames.
- [ ] Modelo de receitas, qualidade e aprimoramentos.
- [ ] Tipos e distribuição de materiais.
- [ ] Inventário sombrio: momento de aprendizado e interface.
- [ ] Progressão de cada elemento.
- [ ] Desbloqueio das formas de Nero.
- [ ] Regras de encontros aleatórios.
- [ ] Sistema de recompensas e economia.
- [ ] Escopo de mapas e duração.

### 21.3. Arte e produção

Os itens abaixo precisam de definição visual, sonora ou técnica antes de serem tratados como
entregas aprovadas.

- [ ] Design de Lucy em cada faixa etária do jogo.
- [ ] Uniforme/aparência dos aprendizes da guilda.
- [ ] Turnarounds definitivos de Nero nas três formas.
- [ ] Design da forma meio-sombra.
- [ ] Visual dos instrutores.
- [ ] Cenários e biomas.
- [ ] Identidade musical e efeitos sonoros.
- [ ] Plataformas, engine e requisitos técnicos.

### 21.4. Critérios para considerar a pré-produção consolidada

**[PROPOSTA]** A lista abaixo propõe evidências para avaliar a pré-produção; os itens ainda não
representam resultados alcançados.

- [ ] Sinopse e linha do tempo aprovadas.
- [ ] Estrutura da campanha e exame aprovados.
- [ ] Loop principal prototipado.
- [ ] Trilha de forja prototipada.
- [ ] Pelo menos uma atividade administrativa divertida.
- [ ] Papel de Nero validado em gameplay.
- [ ] Progressão antes/depois do exame definida.
- [ ] Direção de arte das versões infantis aprovada.
- [ ] Escopo de lançamento e cronograma definidos.

---

## Resumo executivo

**Lucy & Nero — Little Garden** é o primeiro jogo da franquia e acompanha Lucy como aprendiz da
Guilda dos Aventureiros, ao lado de Nero. A experiência gira em torno de **pequenas aventuras**,
**exploração**, **coleta**, **minigames de forja**, **treinamento** e **tarefas administrativas**.
Lucy começa sem dominar magia elemental, embora possua uma reserva de mana equivalente à de Nero.
Ela já aprende sombras com o companheiro antes de seu exame.

O **exame da guilda**, por volta dos 12 anos, revela afinidade com **todos os elementos conhecidos**
e com as **sombras**, cuja existência como elemento passa a ser pública. Depois disso, Lucy aprende
magia com instrutores de cada elemento, enquanto Nero continua responsável pelo ensino das sombras.
O jogo mostra o crescimento dos protagonistas e prepara o universo para as próximas histórias, **sem
revelar a habilidade inata Forjadora de Mundos**, reservada para _Entre Espadas e Garras_.

> **Regra de desenvolvimento:** propostas neste documento só se tornam cânone ou escopo definitivo
> após aprovação explícita.
