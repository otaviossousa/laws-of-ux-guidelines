# Lei de Jakob (Jakob's Law)

> Os usuários passam a maior parte do tempo em *outros* sites e sistemas. Por isso, preferem que o seu funcione da mesma forma que os que eles já conhecem.

**Categoria:** Princípios de sistema · **Relacionadas:** [Modelo Mental](../02-cognicao-e-memoria/modelo-mental.md), [Lei da Similaridade](../01-percepcao-visual/lei-da-similaridade.md)

## Por que importa
O usuário transfere expectativas de produtos familiares para qualquer produto que pareça similar. Aproveitando esses modelos mentais, ele foca na tarefa em vez de aprender uma interface nova. Originalidade em padrões básicos (navegação, formulários, carrinho) costuma custar usabilidade.

## Regras
- **DEVE** usar padrões e convenções consolidados: logo no canto superior esquerdo leva ao início, busca com lupa, carrinho no canto superior direito, links sublinhados, `X` fecha modal, `Esc` fecha overlays.
- **DEVE** usar componentes nativos ou bibliotecas consagradas (inputs, selects, date pickers) em vez de reinventar.
- **DEVE**, ao fazer mudanças grandes (redesign), permitir transição gradual: prévia opcional, coleta de feedback e opção de voltar à versão anterior por um período.
- **NÃO DEVE** mudar o comportamento esperado de controles comuns (ex.: checkbox que se comporta como botão, rolagem sequestrada).
- **NÃO DEVE** inovar em padrões básicos sem evidência de que a novidade é claramente melhor.

## Como aplicar
- Estude 3–5 produtos líderes do mesmo segmento antes de desenhar um fluxo.
- Controles de formulário imitam seus equivalentes físicos (toggle = interruptor, radio = seleção única).
- Em redesigns, lance com feature flag e opção "Usar versão antiga" temporária.
- Siga as diretrizes da plataforma (Material Design no Android, Human Interface Guidelines no iOS).

## Checklist
- [ ] Os padrões de navegação e controles seguem convenções conhecidas?
- [ ] Algum componente foi reinventado sem necessidade?
- [ ] Mudanças grandes têm plano de transição para usuários atuais?

## Origem
Formulada por Jakob Nielsen, cofundador do Nielsen Norman Group e criador da avaliação heurística.

**Fonte:** https://lawsofux.com/jakobs-law/
