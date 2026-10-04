Menu lateral global, fixo à esquerda, com os cinco destinos que existem em todas as telas de Aluno e Professor.

**O consumidor fornece:** o nome do perfil ("Portal do Aluno", "Portal do Professor"), os itens e o contador de não lidos da Central de Avisos.

- Os cinco itens são **sempre** os mesmos e na mesma ordem: Início, Minhas Disciplinas, Central de Avisos, Calendário, Perfil. A Secretaria acessa a gestão a partir do Painel (S01).
- Todo item tem ícone **e** rótulo visível. Não use menu só de ícones.
- O item da página atual leva `aria-current="page"` e fundo `primary`.
- Largura fixa `sidebar-width` (248px); fundo `primary-deep`. Foco usa o anel branco.
- Contador usa `alert` com número; leitor de tela recebe `aria-label`.
- No topo, a logo da marca (`kernel-logo-escuro.svg`, 28px de altura) e abaixo o nome do perfil. Ver a seção Marca.
