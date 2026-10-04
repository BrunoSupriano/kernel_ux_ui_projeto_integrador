# Status e feedback

Mapa único de estados para todas as telas. Cada status tem sempre **componente + ícone + palavra**.

## Status de entrega e atividade

| Status | Selo | Onde aparece | Observação |
|---|---|---|---|
| Pendente | `Badge` pendente (relógio) | A01, A07, A08, P09 | Prazo ainda aberto. |
| Entregue | `Badge` entregue (check) | A07, A08.2, P09 | Vem com comprovante com data e hora. |
| Atrasada | `Badge` atrasada (alerta) | A01, A07, P09 | Único uso do vermelho em lista. |
| Corrigida | `Badge` corrigida (check cheio, fundo `primary`) | A07, A09, P09 | Nota publicada. |

## Status de publicação (Professor)

| Status | Selo | Onde |
|---|---|---|
| Rascunho | `Badge` rascunho | P05, P06, P12 |
| Agendado | `Badge` agendado, com data | P05, P06 |
| Publicado | sem selo; aparece na lista do aluno | P05 |
| Oculto | `Switch` "Visível" desligado + ícone de olho cortado | P05 |

## Status de leitura

- Não lido: ponto cheio `primary`, título em peso 800 e selo "Novo".
- Lido: círculo vazio e título em peso 500.

## Sala e horário

- Alteração recente: selo `Badge` "Sala alterada" em âmbar, banner `Alert` de aviso na tela inicial até o aluno ver, e item destacado no `Timeline` de A11.
- Alteração crítica não pode ser desligada nas preferências (G03).

## Mensagens de feedback

| Situação | Componente | Texto de exemplo |
|---|---|---|
| Salvou / publicou | `Toast` | "Conteúdo publicado e 42 alunos notificados" |
| Entrega concluída | `Alert` sucesso | "Entrega recebida em 07/10, às 21:14" |
| Falha de envio | `Alert` erro | "Não foi possível enviar o arquivo. Ele passa de 20 MB." |
| Campo inválido | texto de erro no campo | "O prazo precisa ser posterior a hoje." |
| Ação destrutiva | `Modal` | "Excluir este conteúdo? Ele sai da sala dos alunos." |
| Salvamento automático | `Autosave` | "Salvo automaticamente às 14:02" |
