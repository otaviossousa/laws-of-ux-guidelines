# Lei de Postel (Postel's Law / Princípio da Robustez)

> Seja liberal no que você aceita e conservador no que você envia.

**Categoria:** Princípios de sistema · **Relacionadas:** [Lei de Tesler](lei-de-tesler.md), [Lei de Parkinson](../04-interacao-e-performance/lei-de-parkinson.md)

## Por que importa
Usuários digitam de formas variadas, usam dispositivos variados e têm capacidades variadas. Um sistema robusto aceita essa variação, interpreta a intenção e devolve uma saída limpa, consistente e previsível. Quanto mais variações forem antecipadas, mais resiliente é o design.

## Regras
- **DEVE** aceitar formatos variados de entrada e normalizá-los (telefone com ou sem máscara, datas com `/` ou `-`, valores com `,` ou `.`, espaços extras, maiúsculas/minúsculas).
- **DEVE** definir limites claros para a entrada e dar feedback compreensível quando ela é inválida.
- **DEVE** ser consistente e previsível na saída (formatos padronizados de data, moeda, números).
- **DEVE** funcionar em diferentes dispositivos, tamanhos de tela, métodos de entrada (mouse, toque, teclado, leitor de tela) e conexões lentas.
- **NÃO DEVE** rejeitar uma entrada cujo significado é claro só porque o formato é diferente do esperado.

## Como aplicar
```js
// Aceitar "(11) 98765-4321", "11987654321", "+55 11 98765 4321"
const normalizarTelefone = (v) => v.replace(/\D/g, '').replace(/^55(?=\d{10,11}$)/, '');

// Aceitar "1.234,56", "1234,56", "1234.56"
const parseValor = (v) => Number(v.trim().replace(/\.(?=\d{3}(\D|$))/g, '').replace(',', '.'));
```
- Busca tolerante: ignorar acentos e caixa, aceitar erros de digitação (fuzzy search).
- E-mail: aplicar `trim()` e converter para minúsculas antes de validar.
- Validação no servidor sempre, mesmo com validação no cliente.

## Checklist
- [ ] Os campos aceitam variações comuns de formato?
- [ ] As mensagens de erro explicam o formato esperado com um exemplo?
- [ ] A saída do sistema é sempre formatada de forma padronizada?
- [ ] A interface funciona com teclado, toque, leitor de tela e telas pequenas?

## Origem
Formulada por Jon Postel, pioneiro da Internet, como diretriz de robustez na especificação do TCP.

**Fonte:** https://lawsofux.com/postels-law/
