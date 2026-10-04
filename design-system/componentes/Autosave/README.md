Indicador de salvamento automático de rascunhos, usado nos editores de plano, conteúdo, atividade e aviso (FT04).

**O consumidor fornece:** o estado atual (`salvo`, `salvando`, `erro`) e o horário do último salvamento.

- Fica perto do título do editor. Mostra **sempre** o horário do último salvamento, para o usuário confiar.
- O erro diz o motivo e deixa o botão "Salvar rascunho" disponível para tentar de novo.
- `role="status"`: anuncia a mudança sem mover o foco.