# Guia por Componente

Quais leis aplicar ao desenhar cada tipo de tela ou componente, com as regras mais importantes resumidas. Siga os links para os detalhes.

---

## Formulários
**Leis-chave:** [Proximidade](../leis/01-percepcao-visual/lei-da-proximidade.md) · [Chunking](../leis/02-cognicao-e-memoria/chunking.md) · [Postel](../leis/05-principios-de-sistema/lei-de-postel.md) · [Parkinson](../leis/04-interacao-e-performance/lei-de-parkinson.md) · [Tesler](../leis/05-principios-de-sistema/lei-de-tesler.md) · [Gradiente de Objetivo](../leis/03-decisao-e-motivacao/efeito-gradiente-de-objetivo.md) · [Fitts](../leis/04-interacao-e-performance/lei-de-fitts.md)

- Label acima do campo, mais perto do seu input do que do anterior.
- Campos agrupados por assunto (Dados pessoais, Endereço, Pagamento); formulários longos viram wizard com progresso ("Etapa 2 de 4").
- Peça apenas o necessário; use `autocomplete`, `inputmode`, CEP → endereço, defaults inteligentes.
- Aceite formatos variados (máscaras opcionais, `,` ou `.`), normalize no código.
- Validação inline ao sair do campo; mensagem de erro junto ao campo, dizendo o que fazer.
- Ao enviar com erros, mova o foco para o primeiro campo inválido.
- Botão de envio próximo ao último campo, com estado de carregamento e proteção contra duplo clique.
- Um botão primário ("Salvar pedido"); "Cancelar" como secundário.
- Salve rascunho automaticamente em formulários longos.

## Navegação e menus
**Leis-chave:** [Jakob](../leis/05-principios-de-sistema/lei-de-jakob.md) · [Hick](../leis/03-decisao-e-motivacao/lei-de-hick.md) · [Posição Serial](../leis/02-cognicao-e-memoria/efeito-de-posicao-serial.md) · [Modelo Mental](../leis/02-cognicao-e-memoria/modelo-mental.md) · [Memória de Trabalho](../leis/02-cognicao-e-memoria/memoria-de-trabalho.md) · [Similaridade](../leis/01-percepcao-visual/lei-da-similaridade.md)

- Siga as convenções: logo leva ao início, perfil/configurações no canto superior direito, menu lateral em sistemas com muitos módulos.
- Itens nomeados pelo objetivo do usuário, não pelo nome técnico do módulo.
- Itens mais importantes no início e no fim; agrupe o resto por categoria.
- Indique sempre onde o usuário está: item ativo destacado, breadcrumbs, título da página.
- Mobile: tab bar inferior com 3–5 itens, com ícone **e** rótulo.

## Tabelas e listas de dados
**Leis-chave:** [Região Comum](../leis/01-percepcao-visual/lei-da-regiao-comum.md) · [Fitts](../leis/04-interacao-e-performance/lei-de-fitts.md) · [Sobrecarga de Escolha](../leis/03-decisao-e-motivacao/sobrecarga-de-escolha.md) · [Fluxo](../leis/04-interacao-e-performance/fluxo.md) · [Doherty](../leis/04-interacao-e-performance/limiar-de-doherty.md) · [Similaridade](../leis/01-percepcao-visual/lei-da-similaridade.md)

- Busca, filtros e ordenação visíveis no topo; mostrar contagem de resultados.
- Linha com hover/zebra; linha inteira clicável para abrir o detalhe.
- Ações em lote (selecionar várias → ação) e edição inline para usuários frequentes.
- Status com badges consistentes (mesma cor + texto em todo o sistema).
- Números alinhados à direita e formatados; datas em formato único.
- Paginação ou virtualização; skeleton durante carregamento.
- Estado vazio que explica e oferece a próxima ação.

## Dashboards
**Leis-chave:** [Pareto](../leis/05-principios-de-sistema/principio-de-pareto.md) · [Carga Cognitiva](../leis/02-cognicao-e-memoria/carga-cognitiva.md) · [Chunking](../leis/02-cognicao-e-memoria/chunking.md) · [Von Restorff](../leis/01-percepcao-visual/efeito-von-restorff.md) · [Prägnanz](../leis/01-percepcao-visual/lei-de-pragnanz.md) · [Atenção Seletiva](../leis/02-cognicao-e-memoria/atencao-seletiva.md)

- Comece com os 3–5 indicadores que respondem às perguntas mais importantes; detalhe sob demanda.
- Agrupe blocos por pergunta de negócio.
- Destaque apenas o que exige ação (alertas, metas em risco).
- Gráficos simples: sem 3D, poucas grades, cores consistentes por série.
- Não faça blocos importantes parecerem banners.

## Botões e ações
**Leis-chave:** [Fitts](../leis/04-interacao-e-performance/lei-de-fitts.md) · [Von Restorff](../leis/01-percepcao-visual/efeito-von-restorff.md) · [Similaridade](../leis/01-percepcao-visual/lei-da-similaridade.md) · [Doherty](../leis/04-interacao-e-performance/limiar-de-doherty.md)

- Mínimo 44×44px de área clicável; ~8px entre alvos.
- Um primário por contexto; variantes com significado fixo (primário, secundário, destrutivo).
- Rótulo com verbo + objeto ("Emitir nota", não "OK").
- Feedback imediato (estado pressionado, spinner no botão).
- Ações destrutivas separadas das frequentes; prefira "Desfazer" a "Tem certeza?" quando a ação for reversível.

## Feedback, carregamento e erros
**Leis-chave:** [Doherty](../leis/04-interacao-e-performance/limiar-de-doherty.md) · [Pico-Fim](../leis/02-cognicao-e-memoria/regra-do-pico-fim.md) · [Atenção Seletiva](../leis/02-cognicao-e-memoria/atencao-seletiva.md) · [Fluxo](../leis/04-interacao-e-performance/fluxo.md)

- < 400 ms para qualquer feedback; skeleton para conteúdo; barra de progresso para processos longos.
- Mensagens perto de onde o usuário está olhando; `aria-live` para leitores de tela.
- Erros em linguagem humana: o que aconteceu + como resolver; nunca só um código técnico.
- Telas de sucesso com próximo passo; capriche no final das jornadas.

## Onboarding e primeiro uso
**Leis-chave:** [Paradoxo do Usuário Ativo](../leis/05-principios-de-sistema/paradoxo-do-usuario-ativo.md) · [Hick](../leis/03-decisao-e-motivacao/lei-de-hick.md) · [Zeigarnik](../leis/02-cognicao-e-memoria/efeito-zeigarnik.md) · [Gradiente de Objetivo](../leis/03-decisao-e-motivacao/efeito-gradiente-de-objetivo.md) · [Pico-Fim](../leis/02-cognicao-e-memoria/regra-do-pico-fim.md)

- Nada de tour longo obrigatório; ensine no contexto, na primeira vez que a função aparece.
- Checklist de primeiros passos com progresso (já começando com algo concluído).
- Libere funções progressivamente.
- Estados vazios que ensinam e oferecem a primeira ação.
- Celebre a primeira conquista (primeiro cadastro, primeira venda).

## Preços, planos e escolhas
**Leis-chave:** [Sobrecarga de Escolha](../leis/03-decisao-e-motivacao/sobrecarga-de-escolha.md) · [Hick](../leis/03-decisao-e-motivacao/lei-de-hick.md) · [Von Restorff](../leis/01-percepcao-visual/efeito-von-restorff.md) · [Viés Cognitivo](../leis/02-cognicao-e-memoria/vies-cognitivo.md)

- 3–4 opções, com a recomendada destacada.
- Tabela de comparação lado a lado.
- Sem dark patterns: nada de urgência falsa, custos ocultos ou opções pré-marcadas escondidas.

## Redesign e mudanças em sistemas existentes
**Leis-chave:** [Jakob](../leis/05-principios-de-sistema/lei-de-jakob.md) · [Modelo Mental](../leis/02-cognicao-e-memoria/modelo-mental.md) · [Pareto](../leis/05-principios-de-sistema/principio-de-pareto.md) · [Estética-Usabilidade](../leis/01-percepcao-visual/efeito-estetica-usabilidade.md)

- Priorize os fluxos mais usados (dados de uso).
- Ofereça transição: prévia opcional, feedback, opção de voltar por um tempo.
- Teste com usuários reais medindo tarefas, tempo e erros — não só a opinião sobre a aparência.
