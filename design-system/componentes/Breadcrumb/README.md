Trilha de localização que mostra onde a pessoa está dentro do AVA, em todas as telas internas.

**O consumidor fornece:** a lista de ancestrais com link e a página atual.

- Máximo de três níveis: Seção > Disciplina > Tela. Nunca mostre código de turma nem a hierarquia institucional (o breadcrumb de sete níveis do Moodle é o contra-exemplo).
- A página atual não é link e leva `aria-current="page"`.
- Use `nav` com `aria-label` e uma lista ordenada (`ol`).