## Marca

O AVA é o ambiente virtual do **Instituto Kernel**, e usa a marca dele: a logo `kernel_`, em que o sublinhado faz o papel de cursor de terminal. A paleta da marca é a mesma deste sistema (`primary` `#2F6F5E`, `primary-deep` `#18382F`, `alert` `#E3A72F`), então logo e interface se encaixam sem ajuste.

## Qual versão usar

| Onde | Arquivo | Altura ou largura |
| --- | --- | --- |
| Menu lateral (`primary-deep`) | `kernel-logo-escuro.svg` | 28px de altura |
| Login e recuperação de senha (`surface`) | `kernel-logo-instituto-claro.svg` | 160px de largura ou mais |
| Topbar em telas sem menu lateral (`surface-raised`) | `kernel-logo-claro.svg` | 24px de altura |
| Rodapé, e-mail e PDF | `kernel-simbolo-claro.svg` | 24px de altura |
| Favicon e aba do navegador | `favicon.svg` | 16px |
| Impressão em preto e branco | `kernel-logo-preto.svg` | Livre, acima do mínimo |

## Regras

- Mínimo: 80px de largura (logo simples), 140px (com INSTITUTO), 16px (ícone).
- Área de proteção: pelo menos a altura do "k" ao redor.
- Sempre a versão certa para o fundo. Não recolora, não estica, não gira.
- O âmbar do sublinhado só existe na versão `verde`, sobre `primary`. Ele tem 2,8:1 contra `primary`, abaixo dos 3:1 de elementos gráficos, porque é decorativo (o nome "kernel" tem 5,9:1). Não use o âmbar como texto nem sozinho sobre branco.
- Sobre fotos, escureça o fundo antes.

## Contraste da logo (calculado)

| Versão sobre o fundo | Contraste |
| --- | --- |
| `claro`: `kernel` `primary-deep` sobre `surface` | 11,8:1 |
| `claro`: sublinhado `primary` sobre `surface` | 5,5:1 |
| `escuro`: `kernel` branco sobre `primary-deep` | 12,8:1 |
| `escuro`: sublinhado `secondary` sobre `primary-deep` | 4,5:1 |
| `verde`: `kernel` branco sobre `primary` | 5,9:1 |
| `verde`: sublinhado `alert` sobre `primary` | 2,8:1 (decorativo) |

## Ícones da marca e ícones de interface

São dois conjuntos diferentes. Os ícones `k_` em tile são **marca** (app, favicon, avatar). Os ícones de **interface** (menu, botão, status) são os 53 ícones do AVA, de traço 2px, em `currentColor` (componente Icons).

## Animação de abertura

Existe uma animação da marca (`kernel_` digitado por um cursor, com `INSTITUTO` abrindo abaixo). Use só na abertura do login ou no carregamento inicial, uma vez, e respeite `prefers-reduced-motion`. Detalhes no componente Logo Animation.
