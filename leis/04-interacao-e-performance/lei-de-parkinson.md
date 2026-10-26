# Lei de Parkinson (Parkinson's Law)

> Toda tarefa se expande até ocupar todo o tempo disponível.

**Categoria:** Interação e performance · **Relacionadas:** [Limiar de Doherty](limiar-de-doherty.md), [Lei de Postel](../05-principios-de-sistema/lei-de-postel.md)

## Por que importa
O usuário tem uma expectativa de quanto tempo uma tarefa deve levar. Se o sistema faz a tarefa durar mais que isso, a experiência piora. Se faz durar **menos**, a experiência melhora. O objetivo é reduzir a duração real abaixo da esperada.

## Regras
- **DEVE** limitar a duração das tarefas ao que o usuário espera (ou menos).
- **DEVE** usar preenchimento automático e dados já conhecidos para poupar digitação.
- **DEVE** pedir apenas os dados estritamente necessários naquele momento.
- **NÃO DEVE** pedir informação que o sistema já tem ou pode inferir.

## Como aplicar
- Atributos `autocomplete` corretos nos campos (`name`, `email`, `tel`, `postal-code`, `cc-number`…).
- Busca de endereço pelo CEP.
- Checkout como convidado e compra em 1 clique para clientes recorrentes.
- Lembrar a última escolha do usuário (filial, impressora, forma de pagamento).
- Importação de dados (planilha, XML) em vez de digitação manual.

```html
<input name="email" type="email" autocomplete="email" />
<input name="cep" inputmode="numeric" autocomplete="postal-code" />
```

## Checklist
- [ ] Todos os campos têm `autocomplete` e `inputmode` adequados?
- [ ] Algum dado pedido já existe no sistema?
- [ ] A tarefa pode ser concluída em menos passos?

## Origem
Cyril Northcote Parkinson, ensaio humorístico publicado na *The Economist* em 1955, baseado na sua experiência no serviço público britânico.

**Fonte:** https://lawsofux.com/parkinsons-law/
