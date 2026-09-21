# TebasFin — Editor YAML e Gantt

Aplicação estática e autocontida para editar visualmente o cronograma do projeto TebasFin Gestora — Valora.

## Estrutura

```text
tebasfin-gantt/
├── index.html
├── app.js
├── styles.css
├── README.md
└── CONTEXTO_PRODUTO.md
```

- `index.html`: estrutura semântica da interface e política de segurança.
- `app.js`: comportamento do editor, parser YAML, dados iniciais e Gantt.
- `styles.css`: identidade visual, layout responsivo e estados de edição.
- `CONTEXTO_PRODUTO.md`: objetivo, escopo, regras e funcionalidades do produto.

## Executar

Abra `index.html` em um navegador moderno. Não há instalação, compilação, backend ou dependências externas.

## Comportamento dos dados

- O planejamento inicial está incorporado em `app.js`.
- Alterações feitas na interface permanecem durante a sessão atual.
- **Baixar YAML** exporta o planejamento vigente.
- **Restaurar exemplo** volta ao planejamento incorporado.
- Preferências visuais de escala e painéis podem ser mantidas pelo navegador.

## Segurança

- Não há chamadas de rede.
- Não há autenticação, cookies, formulários de credenciais ou redirecionamentos.
- JavaScript e CSS são carregados somente do próprio projeto.
- A Content Security Policy bloqueia conexões externas, objetos incorporados e submissão de formulários.
- O download do YAML ocorre apenas por ação explícita do usuário.

