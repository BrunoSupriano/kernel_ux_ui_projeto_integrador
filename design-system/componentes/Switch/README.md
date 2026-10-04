Interruptor que liga ou desliga uma opção com efeito imediato, como "Visível para os alunos" e as preferências de notificação.

**O consumidor fornece:** `role="switch"`, `aria-checked` e um rótulo de texto que descreve o **estado**, não só a opção.

- Use para efeito imediato (sem botão "Salvar"). Para escolhas que só valem após enviar o formulário, use checkbox.
- O estado nunca é só cor: o texto muda ("Visível" / "Oculto") ou o rótulo explica o que está ligado.
- Item crítico que não pode ser desligado fica `disabled` com dica explicando o porquê.
- Alvo de 40px de altura; o texto também é clicável.