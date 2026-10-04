Animação de abertura da marca: um prompt de terminal digita `> init instituto/kernel`, apaga, e o cursor escreve `kernel_` letra por letra, com `INSTITUTO` abrindo logo abaixo.

**O consumidor fornece:** nada. É autocontida (HTML, CSS e um script curto), sobre `primary`, com Plus Jakarta Sans e IBM Plex Mono.

- **Onde usar:** tela de abertura do login (G01), carregamento inicial do app e vídeo ou apresentação da marca. **Só nesses momentos.** Nas telas de trabalho não há animação decorativa.
- **Rode uma vez.** Em produção toque a sequência uma vez e pare em `kernel_` com `INSTITUTO`. O loop de 4,2s e o botão "Reproduzir de novo" existem só na prévia.
- **Duração:** cerca de 5,5s até a marca completa. Nunca bloqueie o carregamento real para esperar a animação: ela some assim que o app estiver pronto.
- **Movimento reduzido:** com `prefers-reduced-motion: reduce` a marca aparece pronta e o cursor não pisca. Mantenha isso.
- **Leitor de tela:** o título `h1` tem `aria-label="Instituto Kernel"`; o texto digitado e o prompt são `aria-hidden`.
- **Cores:** `primary` de fundo, texto `on-primary`, prompt e `INSTITUTO` em `tint-100` (4,8:1). O cursor `_` em `alert` (2,8:1) é decorativo, igual ao sublinhado da logo `verde`. A versão original usava `tint-200` no prompt (3,5:1); aqui subiu para `tint-100` para passar de 4,5:1.
- A animação reproduz a logo em texto. Para a marca estática use os arquivos do grupo Logo.
