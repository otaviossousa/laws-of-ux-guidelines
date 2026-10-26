# Lei de Prägnanz (Lei da Simplicidade / Boa Forma)

> Diante de imagens ambíguas ou complexas, as pessoas as interpretam da forma mais simples possível, porque é a que exige menos esforço cognitivo.

**Categoria:** Percepção visual (Gestalt) · **Relacionadas:** [Carga Cognitiva](../02-cognicao-e-memoria/carga-cognitiva.md), [Navalha de Occam](../05-principios-de-sistema/navalha-de-occam.md)

## Por que importa
O cérebro busca ordem e simplicidade para não ser sobrecarregado. Formas simples são processadas e lembradas melhor. Interfaces com geometria clara, alinhamento e poucas formas são entendidas mais rápido.

## Regras
- **DEVE** usar formas simples e reconhecíveis em ícones, logos e ilustrações de interface.
- **DEVE** alinhar elementos a um grid; alinhamento cria formas implícitas (colunas, blocos) que o olho simplifica.
- **DEVE** reduzir variações gratuitas: poucos raios de borda, poucos tamanhos de fonte, poucas cores.
- **NÃO DEVE** usar ícones detalhados/ilustrativos em tamanhos pequenos.
- **NÃO DEVE** criar layouts com elementos "soltos" e desalinhados.

## Como aplicar
- Grid de 4 ou 8px para tudo; colunas de layout (12 col. web, 4 col. mobile).
- Escala tipográfica limitada (ex.: 5–6 tamanhos).
- 1–2 valores de `border-radius` no sistema inteiro.
- Ícones de uma única biblioteca, grid 24×24, traço uniforme.
- Gráficos: remover grades, bordas e efeitos 3D desnecessários.

## Checklist
- [ ] Todos os elementos se alinham a um grid?
- [ ] Os ícones são legíveis no menor tamanho usado?
- [ ] O número de estilos (fontes, cores, raios, sombras) está enxuto?

## Origem
Derivada das observações de Max Wertheimer (1910) sobre a percepção de movimento aparente, que deram origem à psicologia Gestalt.

**Fonte:** https://lawsofux.com/law-of-pr%C3%A4gnanz/
