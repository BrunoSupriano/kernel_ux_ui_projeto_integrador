Tabela de dados para entregas (P09), diário de notas (P11), notas do aluno (A09) e lista de alunos (P14).

**O consumidor fornece:** `caption`, cabeçalhos com `scope="col"`, linhas e, na coluna de ação, botões `sm`.

- Cabeçalho em `tint-100`, em maiúsculas pequenas; cada célula em linhas de 52px. Primeira coluna em peso 600.
- Colunas numéricas (notas, pesos) à direita, em `mono` com algarismos tabulares.
- Status sempre em `Badge`, nunca só cor. Linha selecionada: fundo `tint-100` e `aria-selected="true"`.
- Filtros e busca ficam acima da tabela, não dentro do cabeçalho. Em edição em lote (P11), a célula vira `TextField` ao receber foco.
- Tabelas longas rolam dentro do conteúdo com cabeçalho fixo.