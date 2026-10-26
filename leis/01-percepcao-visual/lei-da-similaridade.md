# Lei da Similaridade (Law of Similarity)

> Elementos visualmente parecidos são percebidos como relacionados, mesmo quando estão separados.

**Categoria:** Percepção visual (Gestalt) · **Relacionadas:** [Proximidade](lei-da-proximidade.md), [Efeito Von Restorff](efeito-von-restorff.md), [Lei de Jakob](../05-principios-de-sistema/lei-de-jakob.md)

## Por que importa
Cor, forma, tamanho, orientação e movimento funcionam como "etiquetas" visuais. Se dois elementos têm a mesma aparência, o usuário presume que têm a mesma função. Isso é poderoso para consistência e perigoso quando aplicado sem intenção.

## Regras
- **DEVE** dar a mesma aparência a elementos com a mesma função (todos os links iguais, todos os botões primários iguais).
- **DEVE** diferenciar visualmente links e navegação do texto comum (cor + sublinhado ou outro sinal além da cor).
- **DEVE** usar variantes de componentes com significados fixos (primário, secundário, destrutivo, ghost).
- **NÃO DEVE** estilizar texto estático como link ou botão (ex.: texto azul sublinhado que não é clicável).
- **NÃO DEVE** usar a mesma cor para estados semânticos diferentes (ex.: vermelho para "erro" e para "destaque de marca").

## Como aplicar
- Defina um **design system** com tokens semânticos (`--color-action`, `--color-danger`, `--color-success`) e use cada um apenas no seu significado.
- Ícones da mesma família: mesmo peso de traço, mesmo tamanho, mesmo estilo (outline *ou* filled).
- Em tabelas, status iguais = badges iguais em todas as telas do sistema.
- Em gráficos, a mesma série deve ter a mesma cor em todos os gráficos do dashboard.

## Checklist
- [ ] Tudo que é clicável parece clicável, e nada que não é clicável parece?
- [ ] Componentes com a mesma função têm o mesmo estilo em todo o sistema?
- [ ] Cores semânticas são usadas apenas com o seu significado?
- [ ] A diferenciação não depende **só** de cor (acessibilidade)?

## Origem
Princípio de agrupamento da psicologia Gestalt.

**Fonte:** https://lawsofux.com/law-of-similarity/
