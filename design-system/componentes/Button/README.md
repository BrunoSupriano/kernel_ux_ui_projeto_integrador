Botão de ação com cinco variantes (primária, secundária, ghost, destrutiva e destaque) e três tamanhos.

**O consumidor fornece:** o rótulo (verbo no infinitivo + resultado) e, se quiser, um ícone de 20px antes do texto.

- Use **um** botão `ava-btn--primary` por área de decisão. Ele fica à direita no rodapé de formulários e modais.
- `ava-btn--secondary` é a ação alternativa ("Salvar rascunho", "Ver detalhes"). `ava-btn--ghost` é para "Cancelar" e ações terciárias.
- `ava-btn--danger` só abre ou confirma uma ação destrutiva e sempre é precedido de `Modal` de confirmação.
- `ava-btn--accent` (âmbar) é rara: leva o aluno à alteração de sala/horário dentro de um alerta.
- Altura padrão `control-md` (40px); `--lg` (48px) para a ação principal da página; `--sm` (32px) dentro de tabela.
- Desabilitado: use `disabled` e explique o motivo em texto próximo. Carregando: `aria-busy="true"`, spinner no lugar do ícone, mesma largura.
- Não use dois botões primários lado a lado. Não use botão para navegação simples: use link.