# Atenção Seletiva (Selective Attention)

> Processo de focar a atenção em apenas um subconjunto dos estímulos do ambiente — geralmente os relacionados aos nossos objetivos.

**Categoria:** Cognição e memória · **Relacionadas:** [Efeito Von Restorff](../01-percepcao-visual/efeito-von-restorff.md), [Carga Cognitiva](carga-cognitiva.md)

## Por que importa
Usuários filtram o que não parece relevante para a tarefa atual. O design precisa guiar a atenção, evitar distrações e ajudar a encontrar o que importa. Dois fenômenos são críticos:
- **Cegueira a banners:** usuários ignoram, consciente ou inconscientemente, tudo que parece anúncio, está perto de anúncios ou ocupa posições típicas de anúncios.
- **Cegueira a mudanças:** alterações importantes na interface passam despercebidas quando não há sinais fortes ou quando várias mudanças competem ao mesmo tempo.

## Regras
- **DEVE** posicionar informações e ações importantes no caminho natural do olhar e da tarefa.
- **DEVE** sinalizar mudanças de estado com clareza (mensagem perto do local da ação, realce temporário, foco movido para o resultado).
- **DEVE** usar `aria-live` para anunciar mudanças dinâmicas a leitores de tela.
- **NÃO DEVE** estilizar conteúdo importante como banner/anúncio (faixas coloridas no topo, caixas laterais chamativas).
- **NÃO DEVE** disparar várias mudanças simultâneas que disputam atenção.

## Como aplicar
- Feedback de "salvo com sucesso" perto do botão que foi clicado, ou toast consistente, não um banner distante.
- Erros de formulário: ao enviar, mover o foco para o primeiro campo com erro.
- Alterar um valor que afeta outro (ex.: total do carrinho): realçar brevemente o valor alterado.
- Avisos críticos inline no contexto, não em carrosséis ou laterais.

```html
<div role="status" aria-live="polite">Pedido salvo com sucesso.</div>
```

## Checklist
- [ ] Algo importante parece anúncio ou está em posição de anúncio?
- [ ] Mudanças de estado são visíveis perto de onde o usuário está olhando?
- [ ] Mudanças dinâmicas são anunciadas para tecnologias assistivas?

## Origem
Teorias de meados do século XX: Efeito Coquetel de Cherry (1953), Teoria do Filtro de Broadbent (1958), Modelo de Atenuação de Treisman (1960), entre outras.

**Fonte:** https://lawsofux.com/selective-attention/
