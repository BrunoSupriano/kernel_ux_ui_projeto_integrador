Os 53 ícones de interface do AVA em SVG, mais o arquivo `ava-icones-sprite.svg` com todos num só arquivo. Grade de 24px, traço de 2px, pontas arredondadas, sem preenchimento.

- Os SVGs usam `stroke="currentColor"`: herdam a cor do texto. Para pintar, defina `color` no elemento pai com um token (`var(--primary)`).
- **Atenção:** dentro de `<img src="...">` o SVG não herda a cor e aparece preto. Para colorir, insira o SVG em linha ou use o sprite com `<use>`.
- A versão com traço fixo em `ink` (`#1F2A26`), pronta para arrastar no Figma, não está aqui: está no pacote original `ava-icones` (pasta `svg-tinta`).
- Nomes em português, em minúsculas e com hífen (`seta-direita`, `local-sala`). Galeria completa no componente Icons.
