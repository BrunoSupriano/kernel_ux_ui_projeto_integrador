Abas fixas que dividem uma disciplina em Visão geral, Plano, Conteúdos, Atividades, Notas, Avisos e Sala e Horário.

**O consumidor fornece:** a lista de abas, a aba atual e, se houver pendência, o contador.

- A ordem das abas é **a mesma em todas as disciplinas** e entre Aluno e Professor. O Professor acrescenta Entregas, Diário de notas e Alunos, sempre depois das abas compartilhadas.
- Aba selecionada: texto `primary`, peso 700 e barra inferior de 3px. Nunca só cor: o peso e a barra marcam.
- Use `role="tablist"`, `role="tab"` e `aria-selected`; setas esquerda/direita movem entre abas.
- Contador (`ava-tab__count`) só aparece quando há algo a fazer. Rótulos curtos, sem reticências.