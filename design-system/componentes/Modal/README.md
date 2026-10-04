Janela de confirmação sobre uma película `scrim` para ações irreversíveis, como excluir conteúdo, trocar papéis e publicar notas.

**O consumidor fornece:** pergunta no título, consequência em uma ou duas frases e os dois botões.

- O título é uma pergunta objetiva ("Excluir este conteúdo?"). O corpo diz **o que será perdido** e quem é afetado.
- O botão destrutivo repete o verbo ("Excluir conteúdo"), nunca "OK". "Cancelar" é `ghost` e fica à esquerda dele.
- Prende o foco, fecha com `Esc` e devolve o foco ao botão que a abriu. `role="dialog"` e `aria-modal="true"`.
- Flat: contorno `border-strong`, sem sombra; a separação vem do `scrim`.
- Não use modal para informar sucesso nem para formulários longos.