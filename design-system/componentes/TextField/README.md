Campo de texto de uma linha para login, títulos, datas, números e senhas.

**O consumidor fornece:** `label` visível associada ao `input` (`for`/`id`), dica opcional e, em erro, a mensagem em `ava-fielderr` com `aria-describedby`.

- O rótulo fica **acima** do campo e nunca é substituído pelo placeholder. O placeholder mostra só um exemplo.
- Erro: borda `error` de 2px **mais** ícone **mais** texto que diz o campo e como corrigir. Marque `aria-invalid="true"`.
- Campo somente leitura usa `readonly` (fundo `surface`); campo bloqueado usa `disabled` e uma dica dizendo quem define o valor.
- Senha: botão "Mostrar/Ocultar" com texto, não só ícone. Data: use `type="date"`; o seletor nativo mantém teclado e leitor de tela.
- Campos opcionais levam "(opcional)" no rótulo; os obrigatórios não levam asterisco, para não poluir.
- Largura: preencha a coluna de 640px do formulário. Não use campos de largura mista na mesma linha sem necessidade.