# Memória de Trabalho (Working Memory)

> Sistema cognitivo que guarda e manipula temporariamente as informações necessárias para concluir uma tarefa.

**Categoria:** Cognição e memória · **Relacionadas:** [Carga Cognitiva](carga-cognitiva.md), [Lei de Miller](lei-de-miller.md), [Chunking](chunking.md)

## Por que importa
A memória de trabalho comporta poucos blocos de informação por vez (aproximadamente 4 a 7), e cada bloco se perde em cerca de 20–30 segundos sem reforço. Somos bons em **reconhecer** o que já vimos, mas ruins em **lembrar** informação nova. A interface deve carregar o peso da memória, não o usuário.

## Regras
- **DEVE** colocar o ônus da memória no sistema: levar dados relevantes de uma tela para a próxima.
- **DEVE** preferir reconhecimento a lembrança (listas de seleção, histórico, sugestões, itens recentes).
- **DEVE** indicar claramente o que já foi visto (links visitados, breadcrumbs, itens lidos/não lidos).
- **DEVE** permitir comparação lado a lado em vez de exigir que o usuário memorize valores entre telas.
- **NÃO DEVE** pedir que o usuário digite códigos ou valores que aparecem em outra tela.
- **NÃO DEVE** esconder informação necessária para a decisão atual atrás de outra página/aba.

## Como aplicar
- **Resumo persistente:** em checkouts e wizards, mostrar um resumo lateral do que já foi preenchido.
- **Breadcrumbs** e título da página indicando onde o usuário está.
- **Tabelas de comparação** para planos, produtos, propostas.
- **Recentes/favoritos** em buscas e seleções.
- **Copiar com um clique** para códigos, chaves e IDs.
- Mensagens de erro que indicam **qual** campo e **o que** fazer, exibidas junto do campo.

## Checklist
- [ ] O usuário precisa lembrar algo visto em outra tela para concluir esta?
- [ ] Há indicação de onde ele está e por onde já passou?
- [ ] Itens comparáveis podem ser vistos lado a lado?
- [ ] Seleções usam listas/sugestões em vez de digitação livre quando possível?

## Origem
Termo cunhado por Miller, Galanter e Pribram nos anos 1960; Atkinson e Shiffrin (1968) o associaram ao "armazenamento de curto prazo".

**Fonte:** https://lawsofux.com/working-memory/
