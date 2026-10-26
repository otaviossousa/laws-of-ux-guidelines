# Instruções para Assistentes de IA — Laws of UX

Copie este arquivo (ou referencie-o) no `CLAUDE.md`, `AGENTS.md`, `.cursorrules` ou `.github/copilot-instructions.md` dos seus projetos para que assistentes de IA sigam as leis de UX ao gerar ou revisar interfaces.

## Quando gerar ou alterar uma interface, sempre:

### Layout e percepção
1. Use uma escala de espaçamento fixa (4/8/12/16/24/32/48/64). O espaço dentro de um grupo deve ser menor que o espaço entre grupos. *(Proximidade)*
2. Dê o mesmo estilo a elementos com a mesma função; links e botões devem ser visualmente distintos de texto comum. *(Similaridade)*
3. Agrupe entidades em cards/painéis com no máximo 2 níveis de aninhamento. *(Região Comum)*
4. Mostre sequências com conectores visuais (steppers, timelines). *(Conectividade Uniforme)*
5. Alinhe tudo a um grid; limite tamanhos de fonte, cores, raios e sombras aos tokens do design system. *(Prägnanz)*
6. Tenha **um** botão primário por contexto. Nunca comunique algo só com cor. Respeite `prefers-reduced-motion`. *(Von Restorff)*
7. Desenhe estados de carregamento, vazio e erro com o mesmo cuidado do estado ideal. *(Estética-Usabilidade, Pico-Fim)*

### Conteúdo e cognição
8. Remova elementos que não ajudam a tarefa principal; use divulgação progressiva para opções avançadas. *(Carga Cognitiva, Occam)*
9. Nunca obrigue o usuário a lembrar dados de outra tela: mostre resumos, breadcrumbs, recentes e comparações lado a lado. *(Memória de Trabalho)*
10. Divida conteúdo e formulários longos em blocos com títulos; formate números longos em grupos. *(Chunking, Miller)*
11. Use o vocabulário do usuário e do domínio, nunca nomes de tabelas, campos ou módulos internos. *(Modelo Mental)*
12. Não use dark patterns (urgência falsa, opções escondidas pré-marcadas, custos ocultos). *(Viés Cognitivo)*
13. Mostre feedback perto do ponto de ação e anuncie mudanças dinâmicas com `aria-live`. Não estilize conteúdo importante como banner. *(Atenção Seletiva)*
14. Coloque os itens mais importantes no início ou no fim de listas e menus. *(Posição Serial)*
15. Mostre progresso em tarefas longas e permita retomar de onde parou (autosave, rascunhos). *(Zeigarnik, Gradiente de Objetivo)*

### Decisões
16. Minimize o número de opções simultâneas e destaque a recomendada. *(Hick)*
17. Para listas grandes, ofereça busca, filtros e ordenação; para comparações, visão lado a lado. *(Sobrecarga de Escolha)*

### Interação e performance
18. Áreas clicáveis com no mínimo 44×44px e ≥ 8px entre alvos; labels de checkbox/radio clicáveis; linha/card inteiro clicável. *(Fitts)*
19. Dê feedback em < 400 ms: estado pressionado, spinner no botão, skeleton, UI otimista. Desabilite botões de envio durante a requisição. *(Doherty)*
20. Para usuários frequentes: atalhos de teclado, ações em lote, edição inline e "Desfazer" no lugar de confirmações. *(Fluxo)*
21. Use `autocomplete` e `inputmode` corretos; nunca peça dados que o sistema já tem. *(Parkinson)*

### Princípios de sistema
22. Siga convenções da plataforma e use componentes nativos/consagrados em vez de reinventar. *(Jakob)*
23. Aceite variações de formato na entrada (máscaras, separadores, espaços, maiúsculas) e normalize no código; produza saídas padronizadas. Valide também no servidor. *(Postel)*
24. Faça o sistema assumir cálculos, preenchimentos e regras de negócio. *(Tesler)*
25. Dê acesso mais rápido às funções mais usadas. *(Pareto)*
26. Torne a interface autoexplicativa: textos de ajuda, estados vazios com próxima ação, dicas contextuais. Não dependa de manuais ou tours obrigatórios. *(Usuário Ativo)*

## Ao revisar uma interface
Use [`checklists/revisao-de-interface.md`](checklists/revisao-de-interface.md) e cite a lei violada em cada apontamento, com o link para o arquivo correspondente em [`leis/`](leis/).
