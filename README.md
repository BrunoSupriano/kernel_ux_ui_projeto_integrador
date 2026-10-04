<p align="center">
  <img src="assets/banner-instituto-kernel.png" alt="Instituto Kernel" width="100%">
</p>

<h1 align="center">AVA · Ambiente Virtual de Aprendizagem</h1>

<p align="center">
  <strong>Projeto Integrador: UX e UI</strong> · Centro Universitário UniSatc (SATC)<br>
  Professor <strong>Pierre Possamai da Silva</strong>
</p>

<p align="center">
  <img alt="SATC" src="https://img.shields.io/badge/SATC-Projeto%20Integrador-2F6F5E?style=flat-square">
  <img alt="Disciplina" src="https://img.shields.io/badge/disciplina-UX%20e%20UI-18382F?style=flat-square">
  <img alt="Etapa" src="https://img.shields.io/badge/etapa-1%20Pr%C3%A9--projeto%20%E2%86%92%202%20Figma-E3A72F?style=flat-square">
  <img alt="Acessibilidade" src="https://img.shields.io/badge/WCAG-2.1%20AA-3B8A4F?style=flat-square">
</p>

<p align="center"><em>Escreva o futuro.</em></p>

---

## Sumário

1. [Sobre o projeto](#sobre-o-projeto)
2. [Equipe](#equipe)
3. [Por que este projeto existe](#por-que-este-projeto-existe)
4. [Objetivos](#objetivos)
5. [Público-alvo e personas](#público-alvo-e-personas)
6. [Escopo completo](#escopo-completo)
7. [Fluxos e métricas](#fluxos-e-métricas)
8. [Entregáveis](#entregáveis)
9. [Identidade visual](#identidade-visual)
10. [Design system](#design-system)
11. [Páginas de estado](#páginas-de-estado)
12. [Estrutura do repositório](#estrutura-do-repositório)
13. [Como visualizar](#como-visualizar)
14. [Referências principais](#referências-principais)

---

## Sobre o projeto

Este repositório reúne todo o material do trabalho **"Construção de um AVA (Ambiente Virtual de Aprendizagem)"**, desenvolvido na disciplina de **Projeto Integrador: UX e UI** do **Centro Universitário UniSatc (SATC)**, ministrada pelo professor **Pierre Possamai da Silva**.

O desafio da disciplina é projetar, do zero, um AVA para uma universidade fictícia, "do jeito que sempre sonhamos que ele fosse", partindo das dores reais que sentimos como estudantes em sistemas como Moodle, Brightspace e o Portal UniSatc. O trabalho tem três etapas sequenciais: **Pré-Projeto**, **Projeto no Figma** e **Apresentação Final** ([enunciado completo](docs/escopo/escopo-da-disciplina.md)).

Para dar identidade ao sistema, a equipe criou o **Instituto Kernel**, uma instituição fictícia de ensino superior em engenharia de software, com marca, valores, paleta, animação e um design system próprio.

| | |
| --- | --- |
| **Instituição** | Centro Universitário UniSatc (SATC) |
| **Disciplina** | Projeto Integrador: UX e UI |
| **Professor** | Pierre Possamai da Silva |
| **Título do projeto** | AVA — Ambiente Virtual de Aprendizagem centrado nas tarefas de professores e alunos |
| **Instituição fictícia** | Instituto Kernel |
| **Plataforma-alvo** | Web responsiva (*Mobile First* para o aluno; design system desktop documentado) |

## Equipe

| Integrante |
| --- |
| Ana Laura Vicenzi Dordete |
| Bruno de Moraes Supriano |
| Gabriel Ribeiro Fernandes |
| Octávio da Silva Demos |

## Por que este projeto existe

AVAs e portais acadêmicos são a principal ponte entre instituição, professores e alunos fora da sala de aula. Quando falham, o custo não é estético: o aluno perde prazos e avisos, o professor redigita informação e a secretaria absorve atendimento que deveria ser digital.

O pré-projeto mapeou **quatro problemas recorrentes**:

| # | Problema | Consequência |
| --- | --- | --- |
| **PR1** | Falta de coerência entre módulos (avisos, conteúdos, notas e calendário com padrões diferentes) | Carga cognitiva; o sistema fica imprevisível |
| **PR2** | Arquitetura da informação desalinhada ao modelo mental de professores e alunos | Passos desnecessários em tarefas comuns |
| **PR3** | Duplicidade de locais para a mesma informação (plano de ensino × planejamento de aula) | Redigitação e dúvida sobre a versão oficial |
| **PR4** | Comunicação fragmentada de trocas de sala/horário (e-mail, mural, WhatsApp, verbal) | Insegurança e desinformação |

A evidência local vem do diagnóstico de usabilidade do Portal UniSatc (Cardoso; Fernandes; Silva, 2026), com **118 respostas**: usabilidade e navegação (65 menções), organização das informações (42), problemas no mobile (38), design da interface (32), feedback e autonomia (27) e falta de padronização (17).

A causa comum é a **fragmentação da informação**. Por isso a decisão central de arquitetura é: **uma entidade de dados = um único local de edição e consulta**, com visões diferentes por perfil.

> **Pergunta-problema:** de que forma uma arquitetura da informação centrada nas tarefas de professores e alunos, com fonte única de dados e comunicação centralizada, pode reduzir a fragmentação de informação e o retrabalho em um AVA?

## Objetivos

**Objetivo geral:** propor e prototipar um AVA com arquitetura da informação centrada nas tarefas reais de professores e alunos, eliminando duplicidades e unificando os canais de comunicação.

**Objetivos específicos:**

1. Mapear as dores de professores e alunos por meio de personas, entrevistas e benchmarking.
2. Definir uma arquitetura da informação com fonte única por tipo de conteúdo (plano de ensino/planejamento, avisos, sala e horário, notas).
3. Prototipar os fluxos críticos: publicação de conteúdo, atualização do plano de ensino, notificação de troca de sala/horário, consulta de prazos, entrega de atividade e lançamento de nota.
4. Validar o protótipo com teste de usabilidade, medindo tempo de tarefa, cliques, taxa de sucesso e erro, SUS e SEQ.

## Público-alvo e personas

| Persona | Perfil | Objetivo | Necessidade central |
| --- | --- | --- | --- |
| **Jorge, Professor** | 42 anos, 3 disciplinas em 2 cursos; notebook na maior parte do tempo | Publicar conteúdos, planos e avisos sem repetir cadastro | Um único fluxo de publicação, reaproveitável entre turmas, e liberdade para organizar a sala |
| **Bruno, Aluno** | 20 anos, 6 disciplinas; acessa principalmente pelo celular | Saber, sem esforço, prazos, avisos, notas e mudanças de sala | Um único ponto de verdade, com notificação ativa do que é crítico |
| **Secretaria/Admin** (apoio) | Cadastro acadêmico | Cadastrar cursos, turmas, matrículas, salas e períodos | Importação CSV e gestão de alterações de sala/horário |

Detalhes, grau de validação e citações-síntese: [pré-projeto, seção 3](docs/pre-projeto/pre-projeto-ava.md#3-público-alvo-e-personas). Benchmarking de Moodle, Mentor Web, Brightspace e Portal UniSatc: [seção 4](docs/pre-projeto/pre-projeto-ava.md#4-benchmarking-análise-de-concorrentes).

## Escopo completo

### Premissas

1. **Três perfis:** Aluno, Professor e Secretaria/Admin.
2. **Mobile First:** toda tela do Aluno funciona a partir de 360 px; edição pesada do Professor é otimizada para desktop.
3. **Uma entidade = um local de edição.** Avisos, prazos, aulas, notas e mudanças de sala nascem na disciplina; Central de Avisos, Calendário e Dashboards apenas agregam.
4. **Feedback em toda ação:** confirmação, erro claro e "desfazer" quando possível.
5. **Design system único:** mesmos componentes, mesmo menu e mesmo padrão de fluxo em todas as telas.
6. **Dados acadêmicos por importação CSV** no MVP; integração automática na Fase 2.

### Decisões adotadas (a confirmar com o professor)

| # | Decisão | Premissa adotada |
| --- | --- | --- |
| D1 | Secretaria/Admin no MVP | Entra, com o mínimo necessário (S01–S06) |
| D2 | Frequência (chamada) | Fora do MVP (P15 na Fase 2) |
| D3 | Canais de notificação | In-app + e-mail no MVP; push via PWA na Fase 2 |
| D4 | Fonte das notas | O AVA lança as notas (P10, P11), com importação/exportação CSV |
| D5 | Vídeo | Somente link externo (YouTube, Drive etc.) |
| D6 | Recorte do protótipo no Figma | 24 telas usadas nos fluxos F1 a F6, com prioridade para F5 e F6 |
| D7 | Regras de entrega | Configuradas por atividade em P08 |

### Inventário de telas — 39 no MVP + 3 na Fase 2

| Grupo | Telas do MVP |
| --- | --- |
| **Comuns (6)** | G01 Login · G02 Recuperar senha · G03 Perfil e preferências de notificação · G04 Painel de notificações · G05 Busca global · G06 [Páginas de estado](telas/paginas-de-estado/README.md) |
| **Aluno (13)** | A01 Dashboard · A02 Minhas Disciplinas · A03 Disciplina: visão geral · A04 Plano de Ensino (leitura) · A05 Conteúdos · A06 Visualizador de material · A07 Atividades · A08 Atividade: detalhe e entrega · A09 Notas · A10 Avisos da disciplina · A11 Sala e Horário · A12 Central de Avisos · A13 Calendário consolidado |
| **Professor (14)** | P01 Dashboard · P02 Minhas Disciplinas/Turmas · P03 Disciplina: visão geral · P04 Plano de Ensino: editor e versões · P05 Organização da sala · P06 Publicar conteúdo (fluxo único) · P07 Reaproveitar sala entre turmas · P08 Criar/editar atividade · P09 Entregas · P10 Correção individual · P11 Diário de notas · P12 Avisos · P13 Sala e Horário (editar e histórico) · P14 Lista de alunos |
| **Secretaria/Admin (6)** | S01 Painel · S02 Alterações de sala/horário · S03 Importação CSV · S04 Disciplinas e turmas · S05 Usuários e papéis · S06 Salas e períodos letivos |
| **Fase 2 (3)** | A14 Boletim consolidado · P15 Chamada/frequência · S07 Log de auditoria navegável |

### Funcionalidades transversais

| ID | Funcionalidade |
| --- | --- |
| FT01 | Motor único de notificações (in-app e e-mail; push na Fase 2) |
| FT02 | Controle de acesso por papel e vínculo |
| FT03 | Histórico e versionamento (plano de ensino, sala/horário) |
| FT04 | Rascunho, agendamento e salvamento automático |
| FT05 | Feedback padronizado (sucesso, erro, carregamento, confirmação, desfazer) |
| FT06 | [Design system](design-system/README.md) com contraste e foco de teclado (WCAG 2.1 AA) |
| FT07 | Responsivo / Mobile First, alvos de toque de no mínimo 44 px |
| FT08 | Geração de arquivo .ics |
| FT09 | Armazenamento de arquivos (limite, tipos, varredura básica) |
| FT10 | Auditoria mínima (sala/horário, nota e plano) |

### O que entra, o que fica para depois e o que fica de fora

<table>
<tr><th>Entra no MVP</th><th>Fase 2 (planejado)</th><th>Fora do escopo</th></tr>
<tr valign="top"><td>

**Aluno:** dashboard com aulas, prazos, avisos, notas e alertas de sala; disciplinas e visão geral; leitura do plano de ensino; conteúdos com marcação de visto; entrega com revisão, comprovante e reenvio; notas e devolutivas; avisos por disciplina e Central de Avisos; Sala e Horário com histórico; calendário com exportação .ics; notificações, preferências e busca global.

**Professor:** dashboard de pendências; editor único de plano de ensino com versões; publicação em fluxo único com rascunho e agendamento; organização livre da sala (arrastar e soltar com alternativa por botões); reaproveitamento entre turmas; atividades com regras de entrega; correção com nota e comentário; diário de notas; avisos com confirmação de leitura; alteração de sala/horário com motivo, notificação e histórico; lista de alunos.

**Secretaria/Admin:** importação CSV; cadastro de disciplinas, turmas, salas e períodos; usuários e papéis; alteração de sala/horário em lote.

</td><td>

- Boletim consolidado (A14)
- Chamada/frequência (P15)
- Log de auditoria navegável (S07)
- Notificação push via PWA
- Atividades em grupo
- Integração automática com o sistema acadêmico
- Questionários e provas online
- Fórum de dúvidas por disciplina
- Relatórios e indicadores
- Perfil de Coordenador de curso

</td><td>

- Videoconferência nativa
- Gamificação
- Aplicativo mobile nativo
- Chat e mensagens diretas
- Banco de questões e antiplágio
- Certificados, financeiro e matrícula
- Pacotes SCORM
- Multi-idioma
- Integração com WhatsApp
- Recursos de IA
- Editor e hospedagem de vídeo

</td></tr>
</table>

Rastreabilidade dor → tela e detalhamento de cada página: [pré-projeto, seções 5 a 7](docs/pre-projeto/pre-projeto-ava.md#5-escopo-e-funcionalidades).

## Fluxos e métricas

| # | Fluxo | Tipo | Persona |
| --- | --- | --- | --- |
| F1 | Publicar novo conteúdo | Complementar | Jorge |
| F2 | Atualizar plano de ensino | Complementar | Jorge |
| F3 | Avisar troca de sala/horário | Complementar | Jorge, Secretaria → Bruno |
| F4 | Verificar prazos da semana | Complementar | Bruno |
| **F5** | **Entregar atividade** | **Crítico** | Bruno |
| **F6** | **Lançar nota** | **Crítico** | Jorge |

A validação será por **teste de usabilidade moderado** (mínimo de 5 alunos no celular e 5 professores no notebook), comparando o protótipo com o AVA que cada participante usa hoje. Metas principais: publicar conteúdo em **≤ 2 min**, chegar à sala/horário em **≤ 2 cliques**, **≥ 90%** de sucesso nas tarefas-chave, **SUS ≥ 80** e **SEQ ≥ 6,0**. Detalhes: [seção 8](docs/pre-projeto/pre-projeto-ava.md#8-fluxos-de-usuário-principais) e [seção 10](docs/pre-projeto/pre-projeto-ava.md#10-métricas-de-sucesso). Heurísticas de Nielsen, Gestalt e WCAG aplicadas tela a tela: [seção 9](docs/pre-projeto/pre-projeto-ava.md#9-heurísticas-gestalt-e-acessibilidade-wcag).

## Entregáveis

| Entregável | Onde está | Formato |
| --- | --- | --- |
| 📄 Escopo da disciplina (enunciado) | [docs/escopo/escopo-da-disciplina.md](docs/escopo/escopo-da-disciplina.md) | Markdown |
| 📄 Pré-projeto do AVA (Etapa 1) | [docs/pre-projeto/](docs/pre-projeto/README.md) | Markdown + figuras |
| 🏷️ Sobre a marca e valores | [marca/sobre-a-marca-e-valores.md](marca/sobre-a-marca-e-valores.md) | Markdown |
| ✒️ Logos | [marca/logo/](marca/logo/README.md) | SVG, PNG e rascunhos em HTML |
| 🔣 Símbolo `k_` | [marca/simbolo/](marca/simbolo/) | SVG e PNG |
| 🧩 Ícones da marca | [marca/icones/](marca/icones/README.md) | SVG e PNG (16 a 1024 px) |
| 🎨 Paleta de cores | [marca/paleta/](marca/paleta/README.md) | CSS, JSON e estudos em HTML |
| 🎬 Animação da marca | [marca/animacao/](marca/animacao/README.md) | HTML + GIF |
| 🌐 Kit web e social | [marca/web/](marca/web/) · [marca/social/](marca/social/) | Favicon, manifest, banners |
| 🧱 Design system | [design-system/](design-system/README.md) | Tokens, CSS, 34 componentes, guias |
| ✏️ Ícones de interface | [design-system/icones-interface/](design-system/icones-interface/README.md) | 53 SVGs + sprite |
| 🚧 Páginas de estado | [telas/paginas-de-estado/](telas/paginas-de-estado/README.md) | HTML + PNG |

## Identidade visual

<table>
<tr>
<td width="50%" valign="top">

### Marca

A logo é a palavra `kernel` com um underline: o **cursor de terminal** que diz que o próximo passo ainda vai ser escrito. *Kernel* é o núcleo de um sistema operacional e, em inglês, também significa semente.

**Valores:** núcleo primeiro · aprender fazendo · clareza · colaboração · responsabilidade · evolução contínua.

**Tom de voz:** como um bom mentor — direto, acolhedor, técnico sem ser frio.

→ [Sobre a marca e valores](marca/sobre-a-marca-e-valores.md) · [Logos](marca/logo/README.md) · [Ícones](marca/icones/README.md)

</td>
<td width="50%" valign="top">

### Animação

<img src="marca/animacao/animacao-kernel.gif" alt="Animação da marca kernel_" width="100%">

→ [Abrir a animação](marca/animacao/index.html)

</td>
</tr>
</table>

### Paleta · Verde Sálvia (flat)

| Cor | Token | Hex | Papel |
| --- | --- | --- | --- |
| <img src="marca/paleta/swatches/2F6F5E.png" width="40" height="20" alt="#2F6F5E"> | `primary` | `#2F6F5E` | Marca, botão primário, link, item ativo |
| <img src="marca/paleta/swatches/18382F.png" width="40" height="20" alt="#18382F"> | `primary-deep` | `#18382F` | Menu lateral, toast, foco |
| <img src="marca/paleta/swatches/6FA58F.png" width="40" height="20" alt="#6FA58F"> | `secondary` | `#6FA58F` | Apoio decorativo, gráficos |
| <img src="marca/paleta/swatches/E3A72F.png" width="40" height="20" alt="#E3A72F"> | `alert` | `#E3A72F` | Âmbar: cursor da logo, troca de sala, avisos |
| <img src="marca/paleta/swatches/3B8A4F.png" width="40" height="20" alt="#3B8A4F"> | `success` | `#3B8A4F` | Entregue, concluído |
| <img src="marca/paleta/swatches/B83A3A.png" width="40" height="20" alt="#B83A3A"> | `error` | `#B83A3A` | Erro real e prazo perdido |
| <img src="marca/paleta/swatches/F4F7F5.png" width="40" height="20" alt="#F4F7F5"> | `surface` | `#F4F7F5` | Fundo das telas |
| <img src="marca/paleta/swatches/1F2A26.png" width="40" height="20" alt="#1F2A26"> | `ink` | `#1F2A26` | Texto principal |

A Verde Sálvia venceu três concorrentes (Azul Petróleo, Marinho Institucional e Índigo Sereno), testadas nas mesmas telas: [comparativo e estudos](marca/paleta/README.md).

**Tipografia:** Plus Jakarta Sans (títulos e texto) e IBM Plex Mono (notas e códigos).

## Design system

<p align="center"><img src="design-system/pranchas/previews/fundacoes.png" alt="Fundações do design system" width="760"></p>

Sistema único para Aluno, Professor e Secretaria, que ataca diretamente o **PR1** (falta de padronização). Desktop web, Verde Sálvia, flat, meta **WCAG 2.1 AA** com contraste calculado em cada token.

| | |
| --- | --- |
| **Tokens** | 32 cores · 12 estilos de texto · 8 espaçamentos (base 4 px) · 4 raios · medidas de layout → [tokens.json](design-system/tokens/tokens.json) · [tokens.css](design-system/tokens/tokens.css) |
| **Componentes (34)** | AppShell, Sidebar, Topbar, Breadcrumb, Tabs, Stepper, Button, IconButton, TextField, Textarea, Select, SearchField, ChoiceControls, Switch, FileUpload, Alert, Toast, Modal, Autosave, HelpHint, Badge, Card, Table, Accordion, ContentItem, NoticeList, Timeline, Calendar, Progress, EmptyState, Avatar, Icons, Logo, LogoAnimation → [índice](design-system/README.md#componentes) |
| **Ícones** | 53 ícones de traço 2 px em português → [icones-interface](design-system/icones-interface/README.md) |
| **Guias** | [Acessibilidade](design-system/guias/acessibilidade.md) · [Layout e grade](design-system/guias/layout-e-grade.md) · [Marca](design-system/guias/marca.md) · [Status e feedback](design-system/guias/status-e-feedback.md) |
| **Pranchas** | [Fundações](design-system/pranchas/fundacoes.html) · [Navegação](design-system/pranchas/navegacao.html) · [Formulários](design-system/pranchas/acoes-e-formularios.html) · [Feedback](design-system/pranchas/status-e-feedback.html) · [Dados](design-system/pranchas/exibicao-de-dados.html) · [Ícones](design-system/pranchas/pacote-de-icones.html) |

## Páginas de estado

Tela **G06**: o que o AVA mostra fora do caminho feliz, sempre com uma saída clara.

| | | | |
| --- | --- | --- | --- |
| <img src="telas/paginas-de-estado/previews/404-pagina-nao-encontrada.png" width="200"><br>[404 · Não encontrada](telas/paginas-de-estado/404-pagina-nao-encontrada.html) | <img src="telas/paginas-de-estado/previews/403-sem-permissao.png" width="200"><br>[403 · Sem permissão](telas/paginas-de-estado/403-sem-permissao.html) | <img src="telas/paginas-de-estado/previews/429-muitas-tentativas.png" width="200"><br>[429 · Muitas tentativas](telas/paginas-de-estado/429-muitas-tentativas.html) | <img src="telas/paginas-de-estado/previews/erro-generico.png" width="200"><br>[Erro genérico](telas/paginas-de-estado/erro-generico.html) |
| <img src="telas/paginas-de-estado/previews/500-erro-do-servidor.png" width="200"><br>[500 · Erro do servidor](telas/paginas-de-estado/500-erro-do-servidor.html) | <img src="telas/paginas-de-estado/previews/503-manutencao.png" width="200"><br>[503 · Manutenção](telas/paginas-de-estado/503-manutencao.html) | <img src="telas/paginas-de-estado/previews/401-sessao-expirada.png" width="200"><br>[401 · Sessão expirada](telas/paginas-de-estado/401-sessao-expirada.html) | <img src="telas/paginas-de-estado/previews/sem-conexao.png" width="200"><br>[Sem conexão](telas/paginas-de-estado/sem-conexao.html) |

→ [Detalhes e regras de texto](telas/paginas-de-estado/README.md)

## Estrutura do repositório

```text
kernel_ux_ui_projeto_integrador/
├── README.md                     ← você está aqui
├── assets/                       banner do README
├── docs/
│   ├── escopo/                   enunciado da disciplina
│   └── pre-projeto/              pré-projeto completo (Etapa 1) + figuras do benchmarking
├── marca/
│   ├── sobre-a-marca-e-valores.md
│   ├── logo/                     svg/, png/ e rascunhos/
│   ├── simbolo/                  monograma k_
│   ├── icones/                   ícone k_ em tile (3 formas × 3 cores)
│   ├── paleta/                   cores.css, cores.json, estudos/ e previews/
│   ├── animacao/                 index.html + GIF
│   ├── web/                      favicon, manifest, ícones de PWA
│   └── social/                   banners e prévias para redes
├── design-system/
│   ├── tokens/                   tokens.json + tokens.css
│   ├── componentes/              34 componentes (README, preview.html, preview.png) + bundle.css
│   ├── icones-interface/         53 SVGs + sprite
│   ├── pranchas/                 pranchas de documentação (HTML + PNG)
│   ├── guias/                    acessibilidade, layout, marca, status e feedback
│   └── assets/                   notas de uso dos grupos de assets
└── telas/
    └── paginas-de-estado/        G06: 404, 403, 429, 401, 500, 503, fallback, offline
```

## Como visualizar

Os arquivos `.html` são autônomos: abra direto no navegador (as fontes vêm do Google Fonts). Para servir tudo localmente:

```bash
git clone https://github.com/BrunoSupriano/kernel_ux_ui_projeto_integrador.git
cd kernel_ux_ui_projeto_integrador
python -m http.server 8000
# abra http://localhost:8000/marca/animacao/
```

Para usar o design system em outro projeto, copie `design-system/tokens/tokens.css` e `design-system/componentes/bundle.css` e siga o [README do design system](design-system/README.md#como-usar).

## Referências principais

- CARDOSO, D. M. F.; FERNANDES, E. P.; SILVA, P. P. da. **Design centrado no usuário**: análise de melhoria de UX/UI para o ecossistema digital UniSatc. 2026.
- NIELSEN, J. **Usability engineering**. San Diego: Academic Press, 1993.
- NORMAN, D. **The design of everyday things**. New York: Basic Books, 2013.
- MORVILLE, P.; ROSENFELD, L. **Information architecture for the World Wide Web**. 3. ed. O'Reilly, 2006.
- ISO 9241-110:2020 e ISO 9241-210:2019.
- W3C. **Web Content Accessibility Guidelines (WCAG) 2.1**. 2018.
- WROBLEWSKI, L. **Mobile first**. A Book Apart, 2011.

Lista completa no padrão da disciplina: [pré-projeto, seção 12](docs/pre-projeto/pre-projeto-ava.md#12-referências).

---

<p align="center">
  <img src="marca/simbolo/png/kernel-simbolo-claro-512w.png" alt="k_" width="48"><br>
  <sub>Projeto acadêmico · SATC · Projeto Integrador: UX e UI · 2026<br>O Instituto Kernel é uma instituição fictícia criada para este trabalho.</sub>
</p>
