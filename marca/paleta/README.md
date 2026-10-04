# Paleta de cores

[← Marca](../README.md) · [README principal](../../README.md)

A equipe comparou **quatro paletas** aplicadas às mesmas telas (ficha, Dashboard do Aluno, cartaz e estudo de estilos). A escolhida foi a **03 · Verde Sálvia**, em estilo **flat**, que virou a paleta da marca e do design system.

<p align="center"><img src="previews/paleta-final-design-system.png" alt="Paleta final do design system" width="760"></p>

## Arquivos

| Arquivo | Uso |
| --- | --- |
| [cores.css](cores.css) | Variáveis CSS da marca (`--kernel-primary` etc.) |
| [cores.json](cores.json) | Mesmas cores em JSON |
| [tokens.css do design system](../../design-system/tokens/tokens.css) | Todos os tokens de cor, espaço, raio e tipografia do AVA |
| [Paleta final (HTML)](estudos/paleta-final-design-system.html) | 32 cores em blocos chapados, prontas para conta-gotas |

## Paleta final (tokens de cor do AVA)

| Token | Valor | Uso |
| --- | --- | --- |
| <img src="swatches/F4F7F5.png" width="40" height="20" alt="#F4F7F5"> `surface` | `#F4F7F5` | Fundo de página de todas as telas. Texto `ink` e `ink-muted` leem sobre ele (13,7:1 e 6,7:1). |
| <img src="swatches/FFFFFF.png" width="40" height="20" alt="#FFFFFF"> `surface-raised` | `#FFFFFF` | Cards, campos, tabelas, modais e topbar. Fica um degrau acima de `surface`. Texto `ink` 14,8:1; `ink-muted` 7,2:1. |
| <img src="swatches/DFEBE6.png" width="40" height="20" alt="#DFEBE6"> `tint-100` | `#DFEBE6` | Fundo de item selecionado ou em hover, cabeçalho de tabela e badge neutro. Texto `ink` 12,1:1; `primary` 4,8:1. |
| <img src="swatches/B0CEC1.png" width="40" height="20" alt="#B0CEC1"> `tint-200` | `#B0CEC1` | Avatar, contador de aba, evento de calendário de segunda disciplina e área de arrastar ativa. Texto `ink` 8,8:1. |
| <img src="swatches/C9D8D1.png" width="40" height="20" alt="#C9D8D1"> `border` | `#C9D8D1` | Divisores e contornos de card. Decorativo: não é a única pista de um controle. |
| <img src="swatches/6B7F77.png" width="40" height="20" alt="#6B7F77"> `border-strong` | `#6B7F77` | Contorno de campos, checkbox, radio, switch desligado e botão ícone. 4,3:1 sobre `surface-raised` e 3,9:1 sobre `surface` (WCAG 1.4.11). |
| <img src="swatches/1F2A26.png" width="40" height="20" alt="#1F2A26"> `ink` | `#1F2A26` | Texto principal e títulos sobre `surface`, `surface-raised`, `tint-100` e `tint-200`. |
| <img src="swatches/4B5B54.png" width="40" height="20" alt="#4B5B54"> `ink-muted` | `#4B5B54` | Texto secundário (metadados, dicas, rótulos de coluna) sobre `surface`, `surface-raised` e `tint-100`. Mínimo 5,9:1. |
| <img src="swatches/5F7069.png" width="40" height="20" alt="#5F7069"> `placeholder` | `#5F7069` | Texto de exemplo dentro de campo vazio, sobre `surface-raised` (5,2:1). Nunca substitui o rótulo. |
| <img src="swatches/2F6F5E.png" width="40" height="20" alt="#2F6F5E"> `primary` | `#2F6F5E` | Cor da marca: botão primário, link, aba selecionada, item ativo do menu e foco de progresso. Texto `on-primary` sobre ela 5,9:1; como texto sobre `surface-raised` 5,9:1. |
| <img src="swatches/265A4C.png" width="40" height="20" alt="#265A4C"> `primary-hover` | `#265A4C` | Botão primário em hover. `on-primary` sobre ele 7,9:1. |
| <img src="swatches/1D463B.png" width="40" height="20" alt="#1D463B"> `primary-pressed` | `#1D463B` | Botão primário pressionado e hover do menu lateral. |
| <img src="swatches/18382F.png" width="40" height="20" alt="#18382F"> `primary-deep` | `#18382F` | Fundo do menu lateral, toast e texto forte sobre `tint-100`/`tint-200`. `on-primary` sobre ele 12,8:1; `tint-100` 10,4:1. |
| <img src="swatches/FFFFFF.png" width="40" height="20" alt="#FFFFFF"> `on-primary` | `#FFFFFF` | Texto e ícone sobre `primary`, `primary-hover`, `primary-pressed` e `primary-deep`. |
| <img src="swatches/6FA58F.png" width="40" height="20" alt="#6FA58F"> `secondary` | `#6FA58F` | Verde sálvia de apoio: ilustração, faixas decorativas e barras de gráfico. Não use como texto nem como único contorno (2,8:1 sobre branco). |
| <img src="swatches/1F2A26.png" width="40" height="20" alt="#1F2A26"> `on-secondary` | `#1F2A26` | Texto sobre `secondary` (5,3:1). |
| <img src="swatches/E3A72F.png" width="40" height="20" alt="#E3A72F"> `alert` | `#E3A72F` | Âmbar de alerta: selo de contador, fundo do ícone de aviso e botão de destaque. Sempre acompanhado de `on-alert`; nunca sozinho sobre branco (2,1:1). |
| <img src="swatches/1F2A26.png" width="40" height="20" alt="#1F2A26"> `on-alert` | `#1F2A26` | Texto e ícone sobre `alert` (6,9:1). |
| <img src="swatches/D19A28.png" width="40" height="20" alt="#D19A28"> `alert-hover` | `#D19A28` | Botão de destaque em hover. |
| <img src="swatches/FBF0D5.png" width="40" height="20" alt="#FBF0D5"> `alert-tint` | `#FBF0D5` | Fundo de banner de alteração de sala/horário e do selo 'Sala alterada'. |
| <img src="swatches/7A5200.png" width="40" height="20" alt="#7A5200"> `alert-ink` | `#7A5200` | Texto sobre `alert-tint` (6,1:1). |
| <img src="swatches/3B8A4F.png" width="40" height="20" alt="#3B8A4F"> `success` | `#3B8A4F` | Ícone e ponto de sucesso (4,3:1 sobre branco). Para texto ou fundo com texto branco use `success-strong`. |
| <img src="swatches/2F7242.png" width="40" height="20" alt="#2F7242"> `success-strong` | `#2F7242` | Texto de sucesso sobre `surface-raised` e `success-tint` (5,8:1 e 5,0:1) e fundo de barra concluída. |
| <img src="swatches/E2F1E6.png" width="40" height="20" alt="#E2F1E6"> `success-tint` | `#E2F1E6` | Fundo do selo 'Entregue' e do alerta de sucesso. |
| <img src="swatches/B83A3A.png" width="40" height="20" alt="#B83A3A"> `error` | `#B83A3A` | Erro real: borda de campo inválido, botão destrutivo e ícone de erro. Branco sobre ele 5,7:1. Reservado a erro e prazo perdido. |
| <img src="swatches/9E2F2F.png" width="40" height="20" alt="#9E2F2F"> `error-strong` | `#9E2F2F` | Texto de erro sobre `error-tint` (5,9:1) e hover do botão destrutivo. |
| <img src="swatches/F8E3E3.png" width="40" height="20" alt="#F8E3E3"> `error-tint` | `#F8E3E3` | Fundo do selo 'Atrasada' e do alerta de erro. |
| <img src="swatches/18382F.png" width="40" height="20" alt="#18382F"> `focus-ring` | `#18382F` | Anel de foco de teclado (2px) sobre superfícies claras; 12,8:1 sobre branco e 10,4:1 sobre `tint-100`. |
| <img src="swatches/FFFFFF.png" width="40" height="20" alt="#FFFFFF"> `focus-ring-on-dark` | `#FFFFFF` | Anel de foco sobre `primary-deep` (menu lateral e toast). |
| <img src="swatches/E3E9E6.png" width="40" height="20" alt="#E3E9E6"> `disabled-fill` | `#E3E9E6` | Fundo de controle desabilitado. Texto `disabled-ink` é isento de contraste (WCAG 1.4.3), mas o estado também vem com `aria-disabled`. |
| <img src="swatches/6E7D76.png" width="40" height="20" alt="#6E7D76"> `disabled-ink` | `#6E7D76` | Texto e ícone de controle desabilitado. |
|  `scrim` | `rgba(24,56,47,0.6)` | Película atrás de modal. Única transparência do sistema, usada só para separar camadas. |

## Candidatas avaliadas

Ordem das cores: primária, secundária, alerta, sucesso, erro, fundo, texto.

| Paleta | Ideia | Cores | Estudos |
| --- | --- | --- | --- |
| 01 · Azul Petróleo | Sério sem ser frio. Passa confiança acadêmica e funciona bem em estudo prolongado. | `#0F4C5C` `#1F7A8C` `#E09F3E` `#2E7D5B` `#B3261E` `#F4F7F8` `#14232B` | [ficha](estudos/paleta-01-azul-petroleo.html) · [dashboard](estudos/dashboard-paleta-01.html) · [cartaz](estudos/cartaz-paleta-01.html) |
| 02 · Marinho Institucional | A mais formal das quatro. Remete a instituição de ensino consolidada. | `#1B2A4A` `#3D5A99` `#F2A541` `#2F855A` `#C0392B` `#F5F6FA` `#1A1F2E` | [ficha](estudos/paleta-02-marinho-institucional.html) · [dashboard](estudos/dashboard-paleta-02.html) · [cartaz](estudos/cartaz-paleta-02.html) |
| 03 · Verde Sálvia **(escolhida)** | Tom calmo e acolhedor, pensado para quem passa muito tempo olhando a tela. | `#2F6F5E` `#6FA58F` `#E3A72F` `#3B8A4F` `#B83A3A` `#F4F7F5` `#1F2A26` | [ficha](estudos/paleta-03-verde-salvia.html) · [dashboard](estudos/dashboard-paleta-03.html) · [cartaz](estudos/cartaz-paleta-03.html) |
| 04 · Índigo Sereno | Azul com um toque discreto de roxo. Moderna e tecnológica, sem saturação que cansa a vista. | `#3A45A0` `#6B77C4` `#F28F3B` `#2E8B6A` `#C62F2F` `#F6F6FB` `#1C1E33` | [ficha](estudos/paleta-04-indigo-sereno.html) · [dashboard](estudos/dashboard-paleta-04.html) · [cartaz](estudos/cartaz-paleta-04.html) |

| 01 · Azul Petróleo | 02 · Marinho Institucional | 03 · Verde Sálvia | 04 · Índigo Sereno |
| --- | --- | --- | --- |
| <img src="previews/paleta-01-azul-petroleo.png" width="200"> | <img src="previews/paleta-02-marinho-institucional.png" width="200"> | <img src="previews/paleta-03-verde-salvia.png" width="200"> | <img src="previews/paleta-04-indigo-sereno.png" width="200"> |
| <img src="previews/dashboard-paleta-01.png" width="200"> | <img src="previews/dashboard-paleta-02.png" width="200"> | <img src="previews/dashboard-paleta-03.png" width="200"> | <img src="previews/dashboard-paleta-04.png" width="200"> |
| <img src="previews/cartaz-paleta-01.png" width="200"> | <img src="previews/cartaz-paleta-02.png" width="200"> | <img src="previews/cartaz-paleta-03.png" width="200"> | <img src="previews/cartaz-paleta-04.png" width="200"> |

## Estudos de estilo

| Estudo | Prévia |
| --- | --- |
| [O mesmo card em 10 estilos · Marinho](estudos/estudo-estilos-marinho.html) | <img src="previews/estudo-estilos-marinho.png" width="260"> |
| [O mesmo card em 10 estilos · Verde Sálvia](estudos/estudo-estilos-verde-salvia.html) | <img src="previews/estudo-estilos-verde-salvia.png" width="260"> |
| [Dashboard em glassmorfismo (interativo: troca de paleta e desfoque)](estudos/dashboard-glassmorfismo.html) | <img src="previews/dashboard-glassmorfismo-paleta-03.png" width="260"> |

O estilo final é **flat**: superfícies chapadas, sem sombra, sem gradiente e sem desfoque. O glassmorfismo ficou como estudo comparativo.
