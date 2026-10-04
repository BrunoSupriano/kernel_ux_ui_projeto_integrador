Mensagem curta e temporária que confirma o resultado de uma ação, sempre dizendo quem foi notificado.

**O consumidor fornece:** o texto de confirmação e, quando a ação for reversível, o rótulo "Desfazer".

- Uso: salvar, publicar, enviar, lançar nota, alterar sala. Texto no formato "Conteúdo publicado e 42 alunos notificados".
- Fica visível por pelo menos 8 segundos, ou até ser dispensado quando tiver "Desfazer". Aparece no canto inferior esquerdo da área de conteúdo.
- `role="status"`; não rouba o foco.
- Erro nunca vira toast: use `Alert` ou mensagem no campo.