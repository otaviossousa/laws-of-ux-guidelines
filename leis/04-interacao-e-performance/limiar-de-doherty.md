# Limiar de Doherty (Doherty Threshold)

> A produtividade dispara quando computador e usuário interagem num ritmo (abaixo de 400 ms) em que nenhum dos dois precisa esperar pelo outro.

**Categoria:** Interação e performance · **Relacionadas:** [Fluxo](fluxo.md), [Lei de Parkinson](lei-de-parkinson.md), [Regra do Pico-Fim](../02-cognicao-e-memoria/regra-do-pico-fim.md)

## Por que importa
Respostas abaixo de ~400 ms mantêm a atenção e o ritmo de trabalho. Acima disso o usuário começa a "esperar", perde o foco e a sensação de controle. Quando a operação realmente demora, a **performance percebida** (feedback, animação, progresso) faz a espera parecer menor.

## Regras
- **DEVE** dar feedback visual a toda ação em **< 400 ms** (idealmente < 100 ms para cliques/digitação).
- **DEVE** usar UI otimista quando o sucesso é provável (atualiza a tela antes da confirmação do servidor e reverte se falhar).
- **DEVE** usar skeleton screens para carregamentos de conteúdo e barras de progresso para operações longas.
- **DEVE** mostrar progresso determinado (%) para processos acima de ~10 s, com opção de cancelar.
- **PODE** adicionar um atraso intencional em processos que o usuário espera que "deem trabalho" (ex.: busca de melhores preços, análise de segurança) — um resultado instantâneo pode parecer menos confiável.
- **NÃO DEVE** deixar a interface sem resposta depois de um clique (o usuário clica de novo e duplica a ação).

## Como aplicar
| Tempo de resposta | Tratamento |
|---|---|
| < 100 ms | Instantâneo, nenhum indicador necessário |
| 100 ms – 1 s | Estado de "pressionado"/spinner no próprio botão |
| 1 s – 10 s | Skeleton ou spinner com contexto ("Carregando pedidos…") |
| > 10 s | Barra de progresso, estimativa, possibilidade de cancelar ou continuar em segundo plano |

- Desabilitar o botão e mostrar spinner nele ao enviar formulários (evita duplo envio).
- Pré-carregar (prefetch) a próxima tela provável.
- Debounce de 200–300 ms em buscas com digitação.
- Paginação/virtualização em listas grandes.

## Checklist
- [ ] Toda ação tem feedback visual em menos de 400 ms?
- [ ] Carregamentos usam skeleton/progresso em vez de tela em branco?
- [ ] Botões de envio impedem duplo clique?
- [ ] Processos longos podem ser acompanhados e cancelados?

## Origem
Walter J. Doherty e Ahrvind J. Thadani, IBM Systems Journal (1982): reduziram o requisito de tempo de resposta de 2 s para 400 ms.

**Fonte:** https://lawsofux.com/doherty-threshold/
