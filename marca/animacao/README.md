# Animação da marca

[← Marca](../README.md) · [README principal](../../README.md)

<p align="center"><img src="animacao-kernel.gif" alt="Animação de abertura: um prompt digita init instituto/kernel e o cursor escreve kernel_" width="640"></p>

Um prompt de terminal digita `> init instituto/kernel`, apaga, e o cursor âmbar escreve `kernel_` letra por letra. Em seguida, `INSTITUTO` abre embaixo com o espaçamento entre letras se fechando. Fica em loop, com botão "Reproduzir de novo".

- **Arquivo:** [index.html](index.html) (HTML autônomo; abra no navegador). Prévia: [animacao-kernel.gif](animacao-kernel.gif).
- **Uso no AVA:** só na abertura do login ou no carregamento inicial, uma vez. Nas telas de trabalho não há animação decorativa.
- **Acessibilidade:** respeita `prefers-reduced-motion` (mostra a logo pronta, sem movimento) e expõe `aria-label="Instituto Kernel"`.
- Componente correspondente no design system: [LogoAnimation](../../design-system/componentes/LogoAnimation/README.md).
