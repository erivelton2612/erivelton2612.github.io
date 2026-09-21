# TebasFin Gantt — versão estática para GitHub Pages

Aplicação estática do cronograma TebasFin. Não possui autenticação, backend, integrações externas, Google Drive, Render ou acesso a arquivos locais do computador.

## Segurança / funcionamento

- Todos os arquivos são servidos pelo próprio GitHub Pages.
- O único `fetch` carrega `tebasfin_cronograma_macro_padrao.yaml` do mesmo diretório/origem.
- Não usa `showOpenFilePicker`, permissões de filesystem, cookies, formulários externos ou APIs de terceiros.
- Content Security Policy restringe scripts, conexões, imagens e demais recursos à própria origem.
- Alterações feitas no navegador ficam apenas na sessão e podem ser exportadas com **Baixar YAML**.

## Publicação

Envie os arquivos da raiz deste projeto para a raiz do repositório GitHub e ative **Settings → Pages → Deploy from a branch → main → /(root)**.

Arquivos principais: `index.html`, `styles.css`, `app.js`, `tebasfin_cronograma_macro_padrao.yaml` e `.nojekyll`.
