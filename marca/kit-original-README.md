# Kit de marca · Instituto Kernel

Logo escolhida: **kernel_** (Modelo 6), com o underline como cursor de terminal.
Todos os textos dos SVGs estão convertidos em curvas, então não é preciso instalar fonte para usar os arquivos.

## O que tem em cada pasta

| Pasta | Conteúdo | Quando usar |
| --- | --- | --- |
| `logo/` | Logo `kernel_` simples e com `INSTITUTO`, em 5 cores (`verde`, `escuro`, `claro`, `preto`, `branco`). SVG e PNG (800 e 1600 px de largura), fundo transparente | Documentos, slides, site, apresentações |
| `simbolo/` | Monograma `k_` sem fundo, SVG e PNG | Rodapés, marcas d'água, espaços pequenos |
| `icones/` | Ícone `k_` em tile: `arredondado`, `quadrado` e `circulo`, nas cores `verde`, `escuro` e `claro`. PNG de 16 a 1024 px | Apps, repositórios, avatares, ícones de projeto |
| `web/` | `favicon.ico`, `favicon.svg`, `apple-touch-icon.png`, ícones 192/512, maskable, `site.webmanifest`, `head-snippet.html` | Sites e PWAs |
| `social/` | `og-1200x630`, `github-social-preview-1280x640`, `linkedin-banner-1584x396`, `readme-banner-1200x300`, `avatar-400`, `assinatura-email-600w` | Redes, GitHub, e-mail |
| `cores/` | `cores.css` (variáveis CSS) e `cores.json` | Qualquer projeto |

## Qual versão escolher

- Fundo verde `#2F6F5E` (principal): `verde`
- Fundo verde escuro `#18382F`: `escuro`
- Fundo claro: `claro`
- Uma cor só (carimbo, impressão P&B, bordado): `preto` ou `branco`
- Quadrado (`quadrado`) é para lojas de app, apple-touch-icon e ícones maskable; o sistema aplica o arredondamento.

## Uso em projetos de programação

**Site:** copie os arquivos de `web/` para a raiz e cole `head-snippet.html` no `<head>`.

**README do GitHub:**
```md
![Instituto Kernel](social/readme-banner-1200x300.png)
```

**Repositório (Settings → Social preview):** envie `social/github-social-preview-1280x640.png`.

**Variáveis CSS:**
```css
@import "cores/cores.css";
.botao { background: var(--kernel-primary); color: #fff; }
```

**Tipografia:** Plus Jakarta Sans (licença OFL, gratuita), pesos 500 e 800.
```html
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@500;800&display=swap" rel="stylesheet">
```

## Regras de uso

- **Área de proteção:** deixe ao redor da logo pelo menos a altura da letra "k".
- **Tamanho mínimo:** logo simples 80 px de largura; logo com `INSTITUTO` 140 px; ícone 16 px.
- **Âmbar `#E3A72F`:** só no underline da versão `verde`. Não use como texto nem sozinho sobre branco.
- Não estique, não gire, não troque as cores do underline e não coloque a logo sobre fotos sem escurecer o fundo.
