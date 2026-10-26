# Checklist de Revisão de Interface

Use antes de entregar uma tela, em code reviews de front-end ou em revisões de design. Cada item aponta para a lei correspondente.

## Estrutura e percepção
- [ ] Os grupos da tela são identificáveis só pelo espaçamento (espaço interno < espaço entre grupos)? — [Proximidade](../leis/01-percepcao-visual/lei-da-proximidade.md)
- [ ] Elementos com a mesma função têm o mesmo estilo em todo o sistema? — [Similaridade](../leis/01-percepcao-visual/lei-da-similaridade.md)
- [ ] Entidades/seções têm containers claros, com no máximo 2 níveis aninhados? — [Região Comum](../leis/01-percepcao-visual/lei-da-regiao-comum.md)
- [ ] Sequências e fluxos têm conexão visual (stepper, timeline)? — [Conectividade Uniforme](../leis/01-percepcao-visual/lei-da-conectividade-uniforme.md)
- [ ] Tudo está alinhado a um grid e o número de estilos é enxuto? — [Prägnanz](../leis/01-percepcao-visual/lei-de-pragnanz.md)
- [ ] Há exatamente uma ação primária por contexto, destacada com mais de um sinal além da cor? — [Von Restorff](../leis/01-percepcao-visual/efeito-von-restorff.md)
- [ ] Estados vazio, erro e carregamento têm o mesmo acabamento visual do estado ideal? — [Estética-Usabilidade](../leis/01-percepcao-visual/efeito-estetica-usabilidade.md)

## Cognição
- [ ] Cada elemento da tela ajuda a tarefa principal? — [Carga Cognitiva](../leis/02-cognicao-e-memoria/carga-cognitiva.md)
- [ ] O usuário não precisa lembrar nada de outra tela? — [Memória de Trabalho](../leis/02-cognicao-e-memoria/memoria-de-trabalho.md)
- [ ] Conteúdo longo está dividido em blocos com títulos; números longos estão formatados? — [Chunking](../leis/02-cognicao-e-memoria/chunking.md) / [Miller](../leis/02-cognicao-e-memoria/lei-de-miller.md)
- [ ] Rótulos usam o vocabulário do usuário, não termos técnicos? — [Modelo Mental](../leis/02-cognicao-e-memoria/modelo-mental.md)
- [ ] Defaults favorecem o usuário e não há dark patterns? — [Viés Cognitivo](../leis/02-cognicao-e-memoria/vies-cognitivo.md)
- [ ] Nada importante parece anúncio; mudanças de estado são visíveis e anunciadas (`aria-live`)? — [Atenção Seletiva](../leis/02-cognicao-e-memoria/atencao-seletiva.md)
- [ ] Itens mais importantes estão no início ou no fim das listas/menus? — [Posição Serial](../leis/02-cognicao-e-memoria/efeito-de-posicao-serial.md)
- [ ] O fim da jornada (sucesso/erro) é claro, útil e agradável? — [Pico-Fim](../leis/02-cognicao-e-memoria/regra-do-pico-fim.md)
- [ ] Tarefas longas mostram progresso e podem ser retomadas? — [Zeigarnik](../leis/02-cognicao-e-memoria/efeito-zeigarnik.md)

## Decisão
- [ ] O número de opções simultâneas é o mínimo necessário, com uma recomendada? — [Hick](../leis/03-decisao-e-motivacao/lei-de-hick.md)
- [ ] Listas grandes têm busca/filtros; decisões comparativas têm visão lado a lado? — [Sobrecarga de Escolha](../leis/03-decisao-e-motivacao/sobrecarga-de-escolha.md)
- [ ] O usuário sabe quantas etapas faltam? — [Gradiente de Objetivo](../leis/03-decisao-e-motivacao/efeito-gradiente-de-objetivo.md)

## Interação e performance
- [ ] Alvos interativos têm ≥ 44×44px e espaçamento entre si; labels de checkbox são clicáveis? — [Fitts](../leis/04-interacao-e-performance/lei-de-fitts.md)
- [ ] Todo clique tem feedback em < 400 ms; botões de envio evitam duplo clique? — [Doherty](../leis/04-interacao-e-performance/limiar-de-doherty.md)
- [ ] Usuários frequentes têm atalhos, ações em lote e "Desfazer"? — [Fluxo](../leis/04-interacao-e-performance/fluxo.md)
- [ ] Campos têm `autocomplete`/`inputmode`; nenhum dado já conhecido é pedido de novo? — [Parkinson](../leis/04-interacao-e-performance/lei-de-parkinson.md)

## Princípios de sistema
- [ ] Padrões e controles seguem convenções conhecidas da plataforma? — [Jakob](../leis/05-principios-de-sistema/lei-de-jakob.md)
- [ ] Campos aceitam variações de formato e explicam o formato esperado em caso de erro? — [Postel](../leis/05-principios-de-sistema/lei-de-postel.md)
- [ ] Cálculos, preenchimentos e regras ficam com o sistema, não com o usuário? — [Tesler](../leis/05-principios-de-sistema/lei-de-tesler.md)
- [ ] Removi tudo o que podia ser removido sem perder função? — [Occam](../leis/05-principios-de-sistema/navalha-de-occam.md)
- [ ] As funções mais usadas têm o acesso mais rápido? — [Pareto](../leis/05-principios-de-sistema/principio-de-pareto.md)
- [ ] Um usuário novo conclui a tarefa principal sem ler documentação? — [Usuário Ativo](../leis/05-principios-de-sistema/paradoxo-do-usuario-ativo.md)

## Valores de referência rápidos
| Item | Valor |
|---|---|
| Área mínima de toque | 44×44px (iOS), 48×48dp (Android), 24×24px (WCAG 2.2 mínimo) |
| Espaço entre alvos | ≥ 8px |
| Feedback de ação | < 100 ms ideal, < 400 ms máximo |
| Indicador de progresso | Operações > 1 s (spinner/skeleton), > 10 s (barra + cancelar) |
| Contraste de texto (WCAG AA) | 4.5:1 normal, 3:1 grande e componentes |
| Planos de preço | 3–4 opções |
| Itens em tab bar mobile | 3–5 |
| Escala de espaçamento | 4, 8, 12, 16, 24, 32, 48, 64 |
