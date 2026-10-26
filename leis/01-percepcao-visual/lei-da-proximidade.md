# Lei da Proximidade (Law of Proximity)

> Elementos posicionados perto uns dos outros são percebidos como um grupo.

**Categoria:** Percepção visual (Gestalt) · **Relacionadas:** [Região Comum](lei-da-regiao-comum.md), [Similaridade](lei-da-similaridade.md), [Chunking](../02-cognicao-e-memoria/chunking.md)

## Por que importa
O espaço em branco é o recurso de agrupamento mais barato que existe. Antes de ler qualquer texto, o usuário já deduz o que "anda junto" pela distância entre os elementos. Espaçamento errado comunica relações erradas.

## Regras
- **DEVE** usar menos espaço *dentro* de um grupo do que *entre* grupos (regra prática: o espaço externo deve ser pelo menos 2× o interno).
- **DEVE** colocar o rótulo de um campo mais perto do seu input do que do input anterior.
- **DEVE** manter ações próximas do conteúdo que elas afetam (ex.: botão "Editar" dentro do card, não no topo da página).
- **NÃO DEVE** usar espaçamento uniforme em toda a tela — isso apaga a hierarquia.
- **NÃO DEVE** recorrer a bordas/linhas divisórias quando o espaço sozinho já resolve o agrupamento.

## Como aplicar
| Situação | Aplicação |
|---|---|
| Formulários | `label` → 4–8px → `input`; entre campos 16–24px; entre seções 32–48px |
| Cards / listas | Padding interno menor que o gap entre cards |
| Toolbars | Separar grupos de ações (ex.: formatação vs. inserção) com espaço extra |
| Resultados de busca | Título, URL e descrição juntos; espaço maior entre resultados |

Use uma escala de espaçamento fixa (ex.: 4, 8, 12, 16, 24, 32, 48, 64) via tokens para que a hierarquia seja consistente.

```css
.field        { display: grid; gap: var(--space-1); }   /* label + input */
.form-section { display: grid; gap: var(--space-4); }   /* entre campos */
.form         { display: grid; gap: var(--space-8); }   /* entre seções */
```

## Checklist
- [ ] Consigo identificar os grupos da tela olhando-a desfocada (teste do "squint")?
- [ ] Cada rótulo está visivelmente mais perto do seu próprio campo?
- [ ] Botões de ação estão próximos do conteúdo que afetam?
- [ ] O espaçamento segue os tokens da escala?

## Origem
Princípio de agrupamento da psicologia Gestalt (início do século XX), parte do conjunto que explica como percebemos padrões organizados.

**Fonte:** https://lawsofux.com/law-of-proximity/
