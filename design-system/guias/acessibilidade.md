# Acessibilidade

Meta: WCAG 2.1 nível AA em todas as telas, conforme o pré-projeto (seção 9.4).

## Contraste (calculado)

| Par | Contraste |
|---|---|
| `ink` sobre `surface-raised` | 14,8:1 |
| `ink-muted` sobre `surface` | 6,7:1 |
| `on-primary` sobre `primary` | 5,9:1 |
| `on-primary` sobre `primary-deep` | 12,8:1 |
| `on-alert` sobre `alert` | 6,9:1 |
| `alert-ink` sobre `alert-tint` | 6,1:1 |
| `success-strong` sobre `success-tint` | 5,0:1 |
| `error-strong` sobre `error-tint` | 5,9:1 |
| `border-strong` sobre `surface-raised` | 4,3:1 |
| `focus-ring` sobre `surface-raised` | 12,8:1 |

Pares que **não** devem ser usados: `secondary` como texto (2,8:1 sobre branco); `alert` sozinho sobre branco (2,1:1); texto branco sobre `success` (4,3:1, use `success-strong`).

## Cor e significado

- Status sempre com ícone e texto (WCAG 1.4.1). `success-strong` e `error` têm a mesma luminância; nunca dependa da cor para separar "entregue" de "atrasada".
- Calendário: cada disciplina tem rótulo textual no evento; a legenda lista nome e padrão.

## Teclado

- Toda função é alcançável por teclado, inclusive a reordenação de conteúdos (P05), que oferece botões "Mover para cima/baixo" além de arrastar e soltar.
- Ordem de foco segue a leitura. O foco é sempre visível (anel de 2px).
- Menus, abas e modais têm foco gerenciado: aba usa setas; modal prende o foco e fecha com Esc.

## Leitores de tela

- Estrutura semântica: `nav`, `main`, `h1`–`h4` em ordem, `ol` para breadcrumb e etapas, `table` com `caption` e `th scope`.
- Mensagens de status (`Toast`, `Alert`, "Salvo automaticamente") usam `role="status"` ou `role="alert"` e não movem o foco (WCAG 4.1.3).
- Botão de ícone sempre com `aria-label`. Abas usam `role="tablist"`, `role="tab"` e `aria-selected`; a aba atual do menu usa `aria-current="page"`.
- Campo com erro tem `aria-invalid="true"` e `aria-describedby` apontando para a mensagem.

## Tempo e erros

- Sessão avisa antes de expirar e o editor salva sozinho (WCAG 2.2.1).
- Ações irreversíveis (excluir, trocar papel, publicar nota) pedem confirmação ou oferecem "Desfazer" (WCAG 3.3.4).
