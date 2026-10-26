# Modelo Mental (Mental Model)

> Um modelo simplificado, baseado no que achamos que sabemos sobre um sistema e sobre como ele funciona.

**Categoria:** Cognição e memória · **Relacionadas:** [Lei de Jakob](../05-principios-de-sistema/lei-de-jakob.md), [Viés Cognitivo](vies-cognitivo.md)

## Por que importa
O usuário chega com uma ideia de como o sistema deveria funcionar (vinda de outros produtos e do mundo real) e aplica essa ideia ao seu sistema. Quando o design combina com esse modelo, o conhecimento é transferido sem esforço. Quando não combina, surgem erros e frustração. Reduzir a distância entre o modelo mental de quem projeta e o de quem usa é um dos maiores desafios de UX.

## Regras
- **DEVE** usar a linguagem e os conceitos do usuário, não os termos internos do sistema ou do banco de dados.
- **DEVE** seguir convenções do domínio (ex.: e-commerce usa card de produto, carrinho e checkout).
- **DEVE** validar o modelo mental com pesquisa (entrevistas, testes, mapas de jornada, personas).
- **NÃO DEVE** expor a estrutura técnica (tabelas, IDs, estados internos) como estrutura de navegação.
- **NÃO DEVE** presumir que o usuário pensa como a equipe de desenvolvimento.

## Como aplicar
- Nomeie menus e telas pelo **objetivo** do usuário ("Emitir nota", "Cadastrar cliente"), não pelo módulo técnico.
- Use metáforas do mundo real quando ajudarem (pastas, lixeira, carrinho).
- Em sistemas que substituem processos em papel/planilha, mantenha a ordem dos campos e a terminologia que o usuário já conhece.
- Faça *card sorting* para definir a arquitetura de informação.

## Checklist
- [ ] Os rótulos usam o vocabulário do usuário?
- [ ] A estrutura da navegação reflete tarefas, e não a arquitetura técnica?
- [ ] O fluxo foi validado com usuários reais?

## Origem
Proposto pelo psicólogo Kenneth Craik em *The Nature of Explanation* (1943).

**Fonte:** https://lawsofux.com/mental-model/
