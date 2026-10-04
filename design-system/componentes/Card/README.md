Contêiner de conteúdo agrupado, com fundo `surface-raised` e contorno de 1px; a versão clicável leva o aluno à disciplina.

**O consumidor fornece:** título, metadados, selo de status e, em cards de disciplina, os contadores de pendências.

- Flat: sem sombra. O card se separa do fundo pelo degrau `surface` → `surface-raised` e pelo contorno `border`. Hover de card clicável troca o contorno para `primary`.
- Card de disciplina (A02): nome, professor/turma, sala e horário atuais, selo "Sala alterada" se houver, contadores. Sem código técnico de turma.
- O card inteiro é um único link; não aninhe outro link ou botão dentro dele.
- `ava-card--flat` (fundo `tint-100`, sem contorno) destaca um bloco informativo, não um item clicável.
- Padding `space-5`; intervalo entre cards `space-5`.