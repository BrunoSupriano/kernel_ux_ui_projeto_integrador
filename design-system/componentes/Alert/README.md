Banner fixo no corpo da página para avisos importantes, como a alteração de sala/horário no dashboard, o comprovante de entrega e as falhas de envio.

**O consumidor fornece:** variante (`warning`, `info`, `success`, `error`), título curto, texto e, se houver, uma ação.

- **`warning` (âmbar):** alteração de sala/horário e prazos críticos. Fica no topo do dashboard enquanto o aluno não tiver visto. O título diz **o que mudou e quando**.
- `info`: novidade sem urgência. `success`: resultado de uma ação com comprovante. `error`: falha que o usuário precisa corrigir; diga o motivo e a saída.
- Cor + ícone + título + texto. `warning` e `error` usam `role="alert"`; os demais, `role="status"`. Não movem o foco.
- Máximo de um `warning` por tela. Se houver várias alterações, agrupe: "3 alterações de sala".