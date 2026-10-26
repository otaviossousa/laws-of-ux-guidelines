# Efeito Von Restorff (Efeito de Isolamento)

> Quando vários objetos semelhantes estão presentes, aquele que se diferencia dos demais é o mais lembrado.

**Categoria:** Percepção visual · **Relacionadas:** [Atenção Seletiva](../02-cognicao-e-memoria/atencao-seletiva.md), [Similaridade](lei-da-similaridade.md)

## Por que importa
Contraste é o que dirige o olhar. É a base da hierarquia visual: a ação principal deve "saltar" da tela. Mas o efeito só funciona se houver **poucos** elementos destacados — se tudo é destaque, nada é.

## Regras
- **DEVE** destacar visualmente a ação principal de cada tela (um único botão primário por contexto).
- **DEVE** destacar a informação crítica (alertas, totais, plano recomendado).
- **DEVE** comunicar contraste com mais de um canal (cor + ícone + peso/forma), nunca só com cor.
- **DEVE** respeitar `prefers-reduced-motion` ao usar animação para chamar atenção.
- **NÃO DEVE** ter vários elementos competindo por destaque na mesma área.
- **NÃO DEVE** fazer destaques parecerem anúncios (banners chamativos são ignorados — ver *banner blindness* em [Atenção Seletiva](../02-cognicao-e-memoria/atencao-seletiva.md)).

## Como aplicar
- Botão primário preenchido; secundários outline/ghost.
- Tabela de preços: o plano recomendado com borda, badge "Recomendado" e leve elevação.
- Notificações não lidas: ponto/badge + texto em negrito.
- Contraste de texto mínimo WCAG AA: 4.5:1 (texto normal), 3:1 (texto grande e componentes de UI).

```css
@media (prefers-reduced-motion: reduce) {
  .pulse { animation: none; }
}
```

## Checklist
- [ ] Existe exatamente uma ação primária por contexto?
- [ ] O destaque usa mais de um sinal além da cor?
- [ ] Animações respeitam `prefers-reduced-motion`?
- [ ] Nenhum destaque tem cara de anúncio?

## Origem
Estudo de 1933 da psiquiatra Hedwig von Restorff sobre memória de itens isolados em listas.

**Fonte:** https://lawsofux.com/von-restorff-effect/
