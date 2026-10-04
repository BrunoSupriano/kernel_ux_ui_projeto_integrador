Conjunto de 53 ícones de interface do AVA, em grade de 24px, traço de 2px, pontas arredondadas e sem preenchimento.

**O consumidor fornece:** o nome do ícone, o tamanho e um rótulo de texto ou `aria-label`. A cor vem do texto ao redor (`currentColor`).

- **Tamanhos:** 16px em selo e dica, 20px em botão e menu, 24px em ícone de página, 40px dentro de círculo em estado vazio.
- **Cor:** use `ink`, `ink-muted`, `primary` ou a cor do estado (`success-strong`, `error-strong`, `alert-ink`). Nunca um hexadecimal solto.
- **Rótulo:** todo ícone sem texto ao lado leva `aria-label` ou texto oculto (`.ava-sr`). Ícone decorativo leva `aria-hidden="true"`. No menu lateral o ícone nunca vem sem rótulo.
- **Status:** ícone **e** palavra, sempre. `pendente`, `entregue`, `atrasada-erro`, `corrigida` e `sala-alterada` não dependem só da cor.
- **Um nome, um significado.** Cada tipo de conteúdo tem um ícone próprio (`arquivo`, `texto`, `video`, `link`, `atividade`), para nunca repetir o ícone de vídeo e leitura.
- **Uso em código:** o arquivo `ava-icones-sprite.svg` reúne todos (`<use href="ava-icones-sprite.svg#ava-inicio">`). Os SVGs soltos estão no grupo de assets Ícones de interface.
- Não misture com os ícones da marca (`k_`) nem com outra família de traço.
