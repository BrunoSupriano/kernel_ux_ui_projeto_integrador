Botão quadrado só com ícone, usado no sino de notificações, na ajuda, em fechar e em ações de linha.

**O consumidor fornece:** o ícone (20px) e um `aria-label` obrigatório que descreve a ação ("Notificações, 3 não lidas").

- Todo botão de ícone precisa de texto acessível. Para ações que o aluno nunca viu antes, prefira botão com rótulo visível.
- O contador do sino usa `ava-iconbtn__dot` com `alert` e o número, nunca só um ponto sem texto.
- `--plain` remove o contorno e serve para "Fechar" em modal e toast.
- Alvo de 40px (`control-md`). Não reduza.