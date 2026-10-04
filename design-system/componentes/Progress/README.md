Barra de progresso com rótulo e valor em texto, usada em conteúdos vistos, entregas e envio de arquivos.

**O consumidor fornece:** o rótulo, o valor numérico ("7 de 12") e `aria-valuenow`.

- O número sempre aparece em texto ao lado do rótulo; a barra apenas reforça.
- Barra em `primary` enquanto há o que fazer; em `success-strong` quando completa.
- Não use para esperas indeterminadas: use o `ava-spinner` dentro de `Button` ou um `Alert` informativo.