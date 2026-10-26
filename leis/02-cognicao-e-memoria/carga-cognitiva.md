# Carga Cognitiva (Cognitive Load)

> A quantidade de recursos mentais necessária para entender e interagir com uma interface.

**Categoria:** Cognição e memória · **Relacionadas:** [Memória de Trabalho](memoria-de-trabalho.md), [Lei de Miller](lei-de-miller.md), [Chunking](chunking.md), [Lei de Hick](../03-decisao-e-motivacao/lei-de-hick.md)

## Por que importa
Quando a informação que chega excede a capacidade mental disponível, as tarefas ficam difíceis, detalhes passam despercebidos e o usuário se sente sobrecarregado. Existem dois tipos:
- **Carga intrínseca:** o esforço necessário para a tarefa em si (lembrar do objetivo, absorver informação nova). Não dá para eliminar, só apoiar.
- **Carga estranha (extrínseca):** esforço gasto com coisas que não ajudam o usuário (elementos decorativos, distrações, layouts confusos). **Essa deve ser eliminada.**

## Regras
- **DEVE** remover tudo que não ajuda a tarefa atual (decoração, textos redundantes, opções raramente usadas na tela principal).
- **DEVE** usar padrões conhecidos em vez de reinventar componentes (ver [Lei de Jakob](../05-principios-de-sistema/lei-de-jakob.md)).
- **DEVE** dividir tarefas longas em etapas menores (wizards, divulgação progressiva).
- **DEVE** preferir reconhecimento a lembrança: mostrar opções, valores anteriores e contexto em vez de exigir que o usuário lembre.
- **NÃO DEVE** exigir que o usuário faça contas, conversões ou cópias manuais que o sistema poderia fazer.
- **NÃO DEVE** mostrar várias mensagens, modais ou animações ao mesmo tempo.

## Como aplicar
- **Divulgação progressiva:** "Opções avançadas" recolhidas por padrão.
- **Padrões inteligentes (defaults):** pré-preencher com o valor mais provável.
- **Linguagem simples:** rótulos curtos, verbos de ação ("Salvar pedido" em vez de "Ok").
- **Formatação automática:** máscaras de CPF, telefone, moeda.
- **Dashboards:** começar com 3–5 indicadores principais; detalhes sob demanda.

## Checklist
- [ ] Cada elemento da tela ajuda a tarefa principal?
- [ ] O usuário precisa lembrar algo de uma tela anterior? (Se sim, mostre-o.)
- [ ] Tarefas longas estão divididas em etapas?
- [ ] Há cálculos ou formatações que o sistema poderia fazer pelo usuário?

## Origem
Teoria da Carga Cognitiva, desenvolvida por John Sweller no fim dos anos 1980 a partir de estudos sobre resolução de problemas e design instrucional.

**Fonte:** https://lawsofux.com/cognitive-load/
