# Layout e grade

Sistema pensado para **desktop web**: tela mínima de 1024px, base de projeto de 1280px, folga até 1920px.

## Estrutura da página

- **Menu lateral** fixo à esquerda, com `sidebar-width` (248px), fundo `primary-deep`. Cinco itens, iguais em todas as telas de Aluno e Professor: Início, Minhas Disciplinas, Central de Avisos, Calendário, Perfil.
- **Topbar** com `header-height` (64px), fundo `surface-raised` e borda inferior `border`. Contém a busca global à esquerda, o sino de notificações e o perfil à direita.
- **Conteúdo** em `surface`, com margem lateral `space-6` e largura máxima `content-max` (1200px), alinhado à esquerda.
- **Rolagem:** só o conteúdo rola; menu e topbar ficam fixos.

## Grade

- 12 colunas, intervalo (gutter) `space-5` (24px), margem `space-6` (32px).
- Dashboards usam 8 + 4 colunas: lista principal à esquerda (aulas, prazos) e coluna lateral à direita (avisos, notas).
- Listas de cards (Minhas Disciplinas) usam 3 colunas em 1280px e 2 em 1024px.
- Formulários usam coluna única de até 640px, com o resumo ou a prévia numa segunda coluna de 4 colunas quando houver.
- Tabelas ocupam as 12 colunas; as colunas numéricas ficam à direita.

## Pontos de quebra

| Largura | Comportamento |
|---|---|
| 1024–1279px | Layout compacto: 2 cards por linha, coluna lateral do dashboard desce para baixo. |
| 1280–1599px | Layout base. |
| 1600px ou mais | Conteúdo para em `content-max`; margens crescem. |
| Abaixo de 1024px | Fora deste sistema. O pré-projeto prevê versão mobile com barra inferior e alvos de 44px; ela precisa de um conjunto próprio de componentes. |

## Ordem de leitura

1. Título da página e ação principal.
2. Alerta crítico (troca de sala, prazo perdido), quando existir.
3. Conteúdo principal.
4. Coluna lateral.

O urgente aparece primeiro; o secundário vive em abas ou em detalhes expansíveis (Nielsen 8).
