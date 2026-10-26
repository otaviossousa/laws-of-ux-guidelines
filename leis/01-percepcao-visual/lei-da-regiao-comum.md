# Lei da Região Comum (Law of Common Region)

> Elementos que compartilham uma área com limites bem definidos são percebidos como um grupo.

**Categoria:** Percepção visual (Gestalt) · **Relacionadas:** [Proximidade](lei-da-proximidade.md), [Conectividade Uniforme](lei-da-conectividade-uniforme.md)

## Por que importa
Uma borda ou um fundo cria um "container" mental. Isso deixa explícita a relação entre elementos e seções, e é mais forte que a proximidade: um container agrupa itens mesmo que estejam espaçados.

## Regras
- **DEVE** usar cards, painéis ou fundos para agrupar informações que pertencem a uma mesma entidade (ex.: um pedido, um cliente).
- **DEVE** escolher **um** mecanismo principal de container (borda *ou* fundo *ou* sombra) e mantê-lo consistente.
- **NÃO DEVE** aninhar containers em excesso (card dentro de card dentro de card) — cada nível perde força e gera ruído.
- **NÃO DEVE** colocar dentro de um container elementos que não pertencem àquele grupo.

## Como aplicar
| Padrão | Uso |
|---|---|
| Card | Uma entidade com dados + ações (produto, cliente, tarefa) |
| Painel/seção com fundo | Áreas da página (filtros, resumo, detalhes) |
| `fieldset` com borda/fundo | Seções de formulário longas (Dados pessoais, Endereço, Pagamento) |
| Linha zebrada / hover em tabela | Região da linha para leitura horizontal |
| Header/footer de modal | Separar ações do conteúdo |

Prefira no máximo **2 níveis** de containers visíveis em uma tela.

## Checklist
- [ ] Cada entidade/seção tem um limite visual claro?
- [ ] Há no máximo 2 níveis de containers aninhados?
- [ ] O estilo de container é o mesmo em telas equivalentes?

## Origem
Princípio de agrupamento da psicologia Gestalt.

**Fonte:** https://lawsofux.com/law-of-common-region/
