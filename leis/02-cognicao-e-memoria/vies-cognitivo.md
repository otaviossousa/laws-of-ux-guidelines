# Viés Cognitivo (Cognitive Bias)

> Erro sistemático de pensamento ou de julgamento que influencia nossa percepção do mundo e nossa capacidade de decisão.

**Categoria:** Cognição e memória · **Relacionadas:** [Regra do Pico-Fim](regra-do-pico-fim.md), [Efeito de Posição Serial](efeito-de-posicao-serial.md), [Modelo Mental](modelo-mental.md)

## Por que importa
Para economizar energia, usamos atalhos mentais (heurísticas) baseados em experiências passadas. Eles nos tornam rápidos, mas também nos fazem decidir sem perceber as distorções. Isso vale para **usuários** (que decidem dentro da sua interface) e para **a equipe** (que decide o que construir). Conhecer os vieses não os elimina, mas ajuda a identificá-los e a evitar erros e discriminações não intencionais.

## Regras
- **DEVE** projetar escolhas de forma ética: defaults, ordem e enquadramento influenciam decisões — use isso a favor do usuário.
- **DEVE** combater o **viés de confirmação** da equipe: testar hipóteses com dados e usuários reais, buscando evidências contrárias.
- **DEVE** apresentar informações de forma neutra quando a decisão é importante para o usuário (contratos, valores, privacidade).
- **NÃO DEVE** usar *dark patterns* (urgência falsa, opções pré-marcadas escondidas, confirmshaming, custos ocultos).
- **NÃO DEVE** basear decisões de produto em opiniões isoladas ou no caso mais recente.

## Vieses mais relevantes para interfaces
| Viés | Implicação no design |
|---|---|
| Ancoragem | O primeiro valor exibido serve de referência (preços, metas) |
| Efeito default | A maioria mantém a opção pré-selecionada |
| Enquadramento | "90% de sucesso" e "10% de falha" geram decisões diferentes |
| Aversão à perda | Perder pesa mais que ganhar; avisos de perda de dados funcionam |
| Prova social | Avaliações e "mais usado" influenciam escolhas |
| Confirmação (equipe) | Testes devem tentar *refutar* a solução |

## Checklist
- [ ] Os defaults beneficiam o usuário?
- [ ] Há algum padrão manipulativo (dark pattern) no fluxo?
- [ ] A decisão de design foi validada com dados, e não só com opinião?

## Origem
Amos Tversky e Daniel Kahneman introduziram o conceito em 1972, mostrando que o julgamento humano diverge da teoria da escolha racional.

**Fonte:** https://lawsofux.com/cognitive-bias/
