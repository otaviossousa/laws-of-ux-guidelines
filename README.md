<div align="center">

# 🧠 Laws of UX — Diretrizes para Design de Interfaces

**As 30 leis da psicologia aplicada ao design, transformadas em regras práticas para construir sistemas melhores.**

![Leis](https://img.shields.io/badge/leis-30-6366f1?style=for-the-badge)
![Idioma](https://img.shields.io/badge/idioma-PT--BR-22c55e?style=for-the-badge)
![Formato](https://img.shields.io/badge/formato-Markdown-0ea5e9?style=for-the-badge)
![IA Ready](https://img.shields.io/badge/pronto%20para-IA-f59e0b?style=for-the-badge)

[Por que existe](#-por-que-este-repositório-existe) •
[Como usar](#-como-usar) •
[Índice das leis](#-índice-das-leis) •
[Estrutura](#-estrutura) •
[Créditos](#-créditos-e-licença)

</div>

---

## 🎯 Por que este repositório existe

Boas interfaces não são questão de gosto: elas seguem a forma como o cérebro humano **percebe, lembra, decide e age**. O site [lawsofux.com](https://lawsofux.com/), de Jon Yablonski, reúne 30 dessas leis. Só que, no dia a dia do desenvolvimento, uma lista de conceitos não basta. A equipe precisa saber **o que fazer na tela**.

Este repositório converte cada lei em **instruções acionáveis**, para que:

- 👩‍💻 **Desenvolvedores** saibam exatamente qual espaçamento, tamanho de botão, tempo de resposta e comportamento usar.
- 🎨 **Designers** tenham uma referência comum para justificar decisões ("isso viola a Lei de Hick").
- 🔍 **Revisores** tenham um checklist objetivo para aprovar telas antes da entrega.
- 🤖 **Assistentes de IA** (Claude, Copilot, Cursor…) gerem interfaces que já seguem boas práticas de UX.

> **Em resumo:** é o "manual de estilo de UX" para ser usado em todos os nossos sistemas, do primeiro rascunho ao code review.

## ✨ O que foi feito

| | |
|---|---|
| 📚 **30 leis analisadas** | Todas as leis do lawsofux.com, organizadas em 5 categorias |
| ✅ **Regras DEVE / NÃO DEVE** | Cada lei virou um conjunto de regras objetivas |
| 🛠️ **Exemplos práticos** | Valores de referência (px, ms, contraste), trechos de HTML/CSS/JS e casos de sistemas reais |
| ☑️ **Checklist por lei** | Perguntas para validar cada tela |
| 🧩 **Guia por componente** | Quais leis aplicar em formulários, tabelas, menus, dashboards, onboarding… |
| 📋 **Checklist de revisão** | Uma lista única para usar em code reviews e entregas |
| 🤖 **Instruções para IA** | 26 regras prontas para colar em `CLAUDE.md`, `.cursorrules` ou instruções do Copilot |

## 🚀 Como usar

### 1. Desenhando uma tela nova
Abra o [**Guia por Componente**](guias/por-componente.md), encontre o tipo de tela (formulário, tabela, dashboard…) e siga as regras listadas.

### 2. Revisando uma tela antes de entregar
Percorra o [**Checklist de Revisão**](checklists/revisao-de-interface.md). Cada item aponta para a lei que justifica a regra.

### 3. Fazendo a IA seguir as leis nos seus projetos
Copie o conteúdo de [**AGENTS.md**](AGENTS.md) para o arquivo de instruções do assistente que você usa no projeto:

| Ferramenta | Arquivo |
|---|---|
| Claude Code | `CLAUDE.md` |
| Cursor | `.cursorrules` ou `.cursor/rules/` |
| GitHub Copilot | `.github/copilot-instructions.md` |
| Outros agentes | `AGENTS.md` |

### 4. Estudando uma lei a fundo
Navegue pelo [índice abaixo](#-índice-das-leis). Cada arquivo segue a mesma estrutura:

```
📄 Definição  →  💡 Por que importa  →  ✅ Regras  →  🛠️ Como aplicar  →  ☑️ Checklist  →  📖 Origem e fonte
```

## 📚 Índice das leis

### 👁️ 1. Percepção visual: como o usuário *enxerga*
| Lei | Em uma frase |
|---|---|
| [Lei da Proximidade](leis/01-percepcao-visual/lei-da-proximidade.md) | O que está perto é percebido como grupo |
| [Lei da Similaridade](leis/01-percepcao-visual/lei-da-similaridade.md) | O que é parecido é percebido como relacionado |
| [Lei da Região Comum](leis/01-percepcao-visual/lei-da-regiao-comum.md) | O que divide um mesmo container é percebido como grupo |
| [Lei da Conectividade Uniforme](leis/01-percepcao-visual/lei-da-conectividade-uniforme.md) | O que está ligado visualmente parece mais relacionado |
| [Lei de Prägnanz](leis/01-percepcao-visual/lei-de-pragnanz.md) | O olho interpreta tudo da forma mais simples possível |
| [Efeito Von Restorff](leis/01-percepcao-visual/efeito-von-restorff.md) | O que é diferente é lembrado |
| [Efeito Estética-Usabilidade](leis/01-percepcao-visual/efeito-estetica-usabilidade.md) | O que é bonito parece mais fácil de usar |

### 🧠 2. Cognição e memória: como o usuário *pensa e lembra*
| Lei | Em uma frase |
|---|---|
| [Carga Cognitiva](leis/02-cognicao-e-memoria/carga-cognitiva.md) | Elimine o esforço mental que não ajuda a tarefa |
| [Memória de Trabalho](leis/02-cognicao-e-memoria/memoria-de-trabalho.md) | O sistema deve lembrar, não o usuário |
| [Lei de Miller](leis/02-cognicao-e-memoria/lei-de-miller.md) | A memória de curto prazo comporta ~7 (±2) itens |
| [Chunking](leis/02-cognicao-e-memoria/chunking.md) | Divida a informação em blocos significativos |
| [Modelo Mental](leis/02-cognicao-e-memoria/modelo-mental.md) | Desenhe conforme o que o usuário acha que o sistema faz |
| [Viés Cognitivo](leis/02-cognicao-e-memoria/vies-cognitivo.md) | Atalhos mentais distorcem decisões: use-os com ética |
| [Atenção Seletiva](leis/02-cognicao-e-memoria/atencao-seletiva.md) | O usuário ignora o que não parece relevante |
| [Efeito de Posição Serial](leis/02-cognicao-e-memoria/efeito-de-posicao-serial.md) | O primeiro e o último itens são os mais lembrados |
| [Regra do Pico-Fim](leis/02-cognicao-e-memoria/regra-do-pico-fim.md) | A experiência é julgada pelo pico e pelo final |
| [Efeito Zeigarnik](leis/02-cognicao-e-memoria/efeito-zeigarnik.md) | Tarefas incompletas ficam na cabeça |

### ⚖️ 3. Decisão e motivação: como o usuário *escolhe e persiste*
| Lei | Em uma frase |
|---|---|
| [Lei de Hick](leis/03-decisao-e-motivacao/lei-de-hick.md) | Mais opções = decisões mais lentas |
| [Sobrecarga de Escolha](leis/03-decisao-e-motivacao/sobrecarga-de-escolha.md) | Opções demais paralisam |
| [Efeito Gradiente de Objetivo](leis/03-decisao-e-motivacao/efeito-gradiente-de-objetivo.md) | Quanto mais perto do fim, maior a motivação |

### ⚡ 4. Interação e performance: como o usuário *age*
| Lei | Em uma frase |
|---|---|
| [Lei de Fitts](leis/04-interacao-e-performance/lei-de-fitts.md) | Alvos grandes e próximos são mais rápidos de acertar |
| [Limiar de Doherty](leis/04-interacao-e-performance/limiar-de-doherty.md) | Responda em menos de 400 ms |
| [Fluxo](leis/04-interacao-e-performance/fluxo.md) | Equilibre desafio e habilidade; remova fricção |
| [Lei de Parkinson](leis/04-interacao-e-performance/lei-de-parkinson.md) | Faça a tarefa levar menos tempo do que o esperado |

### 🏗️ 5. Princípios de sistema: como *construir* o produto
| Lei | Em uma frase |
|---|---|
| [Lei de Jakob](leis/05-principios-de-sistema/lei-de-jakob.md) | Funcione como os sistemas que o usuário já conhece |
| [Lei de Postel](leis/05-principios-de-sistema/lei-de-postel.md) | Aceite entradas variadas, devolva saídas consistentes |
| [Lei de Tesler](leis/05-principios-de-sistema/lei-de-tesler.md) | A complexidade essencial deve ficar com o sistema |
| [Navalha de Occam](leis/05-principios-de-sistema/navalha-de-occam.md) | A solução mais simples que funciona é a melhor |
| [Princípio de Pareto](leis/05-principios-de-sistema/principio-de-pareto.md) | 20% das funções geram 80% do valor |
| [Paradoxo do Usuário Ativo](leis/05-principios-de-sistema/paradoxo-do-usuario-ativo.md) | Ninguém lê o manual: a ajuda tem que estar na tela |

## 📏 Valores de referência rápidos

| Item | Valor | Lei |
|---|---|---|
| Área mínima de toque | 44×44px (iOS) · 48×48dp (Android) | Fitts |
| Espaço entre alvos clicáveis | ≥ 8px | Fitts |
| Tempo máximo para feedback | < 400 ms | Doherty |
| Barra de progresso | Operações > 10 s, com opção de cancelar | Doherty |
| Contraste de texto (WCAG AA) | 4.5:1 normal · 3:1 grande | Von Restorff |
| Planos de preço | 3–4 opções, uma destacada | Sobrecarga de Escolha |
| Botões primários por contexto | 1 | Von Restorff |
| Escala de espaçamento | 4 · 8 · 12 · 16 · 24 · 32 · 48 · 64 | Proximidade |

## 🗂️ Estrutura

```
laws-of-ux-guidelines/
├── README.md                         ← você está aqui
├── AGENTS.md                         ← regras para assistentes de IA
├── checklists/
│   └── revisao-de-interface.md       ← checklist para revisar telas
├── guias/
│   └── por-componente.md             ← quais leis aplicar em cada componente
└── leis/
    ├── 01-percepcao-visual/          ← 7 leis
    ├── 02-cognicao-e-memoria/        ← 10 leis
    ├── 03-decisao-e-motivacao/       ← 3 leis
    ├── 04-interacao-e-performance/   ← 4 leis
    └── 05-principios-de-sistema/     ← 6 leis
```

## 🙏 Créditos e licença

As leis foram catalogadas por **Jon Yablonski** em [lawsofux.com](https://lawsofux.com/), conteúdo licenciado sob [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/). Recomendo também o livro *Laws of UX* (O'Reilly).

Este repositório **não reproduz** o texto do site. É um material próprio, escrito em português, com interpretações e regras de aplicação prática inspiradas nas leis. Cada arquivo traz o link para a página original.

<div align="center">

**Feito para criar interfaces que respeitam a forma como as pessoas pensam.** 💜

</div>
