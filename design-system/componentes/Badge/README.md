Selo com ícone e palavra que mostra o status de um item: Pendente, Entregue, Atrasada, Corrigida, Rascunho, Agendado, Sala alterada e Novo.

**O consumidor fornece:** o status do dado; o selo escolhe variante, ícone e rótulo.

- **Ícone e texto são obrigatórios.** A cor sozinha nunca diz o status (WCAG 1.4.1); `success-strong` e `error` têm a mesma luminância e só se distinguem pelo ícone e pela palavra.
- Uma lista nunca mistura palavras diferentes para o mesmo status. O vocabulário está em "Status e feedback".
- `ava-badge--changed` (âmbar) é o único selo com contorno colorido: ele precisa chamar atenção.
- Vermelho (`late`) só para prazo perdido e erro real.
- Não use selo para ação: se for clicável, use `Button`.