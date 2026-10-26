# Navalha de Occam (Occam's Razor)

> Entre hipóteses que explicam algo igualmente bem, deve-se escolher a que tem menos suposições.

**Categoria:** Princípios de sistema · **Relacionadas:** [Lei de Tesler](lei-de-tesler.md), [Prägnanz](../01-percepcao-visual/lei-de-pragnanz.md), [Carga Cognitiva](../02-cognicao-e-memoria/carga-cognitiva.md)

## Por que importa
No design, a melhor forma de reduzir complexidade é não criá-la. Entre duas soluções que resolvem o problema igualmente bem, a mais simples é mais fácil de entender, manter, testar e evoluir.

## Regras
- **DEVE** analisar cada elemento da tela e remover tudo que puder ser removido sem prejudicar a função.
- **DEVE** considerar o design pronto apenas quando não houver mais nada que possa ser retirado.
- **DEVE** preferir a solução com menos telas, menos passos, menos componentes e menos estados.
- **NÃO DEVE** adicionar recursos "por precaução" sem evidência de necessidade.
- **NÃO DEVE** confundir simples com incompleto — a função precisa permanecer intacta.

## Como aplicar
- Revisão de tela com a pergunta "e se eu tirar isso?" para cada elemento.
- Um único componente configurável em vez de vários parecidos.
- Um fluxo linear em vez de vários caminhos alternativos para o mesmo resultado.
- No código: menos dependências, menos variações de componentes no design system.

## Checklist
- [ ] Cada elemento tem um motivo claro para existir?
- [ ] Existe uma solução com menos passos que atinge o mesmo resultado?
- [ ] Algum recurso foi adicionado sem necessidade comprovada?

## Origem
Atribuída a Guilherme de Ockham (c. 1287–1347), frade e filósofo inglês — o "princípio da parcimônia".

**Fonte:** https://lawsofux.com/occams-razor/
