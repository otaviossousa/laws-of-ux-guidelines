# Lei de Fitts (Fitts's Law)

> O tempo para alcançar um alvo depende da distância até ele e do seu tamanho.

**Categoria:** Interação e performance · **Relacionadas:** [Limiar de Doherty](limiar-de-doherty.md), [Lei de Hick](../03-decisao-e-motivacao/lei-de-hick.md)

## Por que importa
Alvos pequenos e distantes são lentos e propensos a erro (há um trade-off entre velocidade e precisão). Isso vale para mouse e principalmente para toque. Botões grandes, bem espaçados e próximos de onde a atenção do usuário já está tornam a interação mais rápida e precisa.

## Regras
- **DEVE** ter alvos de toque grandes o suficiente: **mínimo 44×44px** (iOS) / **48×48dp** (Android/Material); WCAG 2.2 exige no mínimo 24×24px.
- **DEVE** espaçar alvos adjacentes (mínimo ~8px) para evitar toques errados.
- **DEVE** posicionar ações próximas do ponto onde o usuário está trabalhando (botão de enviar perto do último campo).
- **DEVE** tornar toda a área visual clicável (linha inteira da lista, card inteiro, label do checkbox).
- **DEVE** posicionar ações frequentes no mobile na zona alcançável pelo polegar (parte inferior da tela).
- **NÃO DEVE** colocar ações destrutivas grudadas em ações frequentes (ex.: "Excluir" ao lado de "Salvar").

## Como aplicar
```css
.btn, .icon-button { min-width: 44px; min-height: 44px; }
.list-item a { display: block; padding: 12px 16px; } /* linha inteira clicável */
```
```html
<label class="checkbox"><input type="checkbox" /> Lembrar de mim</label>
```
- Bordas e cantos da tela são alvos "infinitos" no desktop (menus no topo, docks).
- Menus contextuais (clique direito) aparecem junto do cursor — distância zero.
- Mobile: barra de ações inferior, FAB para ação principal.

## Checklist
- [ ] Todos os alvos interativos têm pelo menos 44×44px (ou 24×24px com espaçamento adequado)?
- [ ] O label de checkbox/radio é clicável?
- [ ] Ações destrutivas estão separadas das frequentes?
- [ ] No mobile, as ações principais estão ao alcance do polegar?

## Origem
Paul Fitts (1954) mostrou que o tempo de movimento até um alvo aumenta com a distância e diminui com o tamanho do alvo.

**Fonte:** https://lawsofux.com/fittss-law/
