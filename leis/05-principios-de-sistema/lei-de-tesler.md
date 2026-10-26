# Lei de Tesler (Lei da Conservação da Complexidade)

> Todo sistema tem uma quantidade de complexidade que não pode ser reduzida.

**Categoria:** Princípios de sistema · **Relacionadas:** [Navalha de Occam](navalha-de-occam.md), [Lei de Postel](lei-de-postel.md), [Paradoxo do Usuário Ativo](paradoxo-do-usuario-ativo.md)

## Por que importa
Todo processo tem um núcleo de complexidade inerente. A única pergunta é **quem** carrega esse peso: o sistema (designers e desenvolvedores) ou o usuário. Gastar uma semana a mais de desenvolvimento para poupar um minuto de milhões de usuários quase sempre compensa.

## Regras
- **DEVE** transferir ao máximo a complexidade para o sistema (cálculos, validações, preenchimentos, regras de negócio).
- **DEVE** projetar para pessoas reais, que nem sempre se comportam de forma racional ou ideal.
- **DEVE** oferecer ajuda contextual (tooltips, textos de apoio, exemplos) onde a complexidade não pôde ser removida.
- **NÃO DEVE** "simplificar" escondendo complexidade necessária de forma que o usuário fique sem controle.
- **NÃO DEVE** empurrar para o usuário decisões técnicas que o sistema pode tomar (formatos, códigos, configurações internas).

## Como aplicar
- Cálculo automático de impostos, frete, totais e datas de vencimento.
- Detecção automática (bandeira do cartão, endereço pelo CEP, fuso horário, idioma).
- Defaults inteligentes + "Avançado" para quem precisa.
- Integrações que eliminam digitação dupla entre sistemas.
- Sabendo que usuários, quando algo fica simples, passam a tentar tarefas mais complexas — planeje a evolução.

## Checklist
- [ ] Qual é a complexidade essencial deste fluxo e quem a está carregando hoje?
- [ ] Há algo que o usuário faz manualmente que o sistema poderia fazer?
- [ ] A complexidade restante tem ajuda contextual?

## Origem
Larry Tesler, na Xerox PARC em meados dos anos 1980; popularizada na entrevista do livro *Designing for Interaction*, de Dan Saffer.

**Fonte:** https://lawsofux.com/teslers-law/
