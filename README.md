# TebasFin — Gantt YAML Editor

Site estático pronto para GitHub Pages. A interface foi preservada a partir do HTML original, com CSS e JavaScript separados e o cronograma inicial extraído para `tebasfin_cronograma_macro_padrao.yaml`.

## Estrutura

- `index.html` — página principal
- `styles.css` — visual original
- `app.js` — editor YAML + Gantt
- `tebasfin_cronograma_macro_padrao.yaml` — cronograma carregado na abertura
- `.nojekyll` — publicação direta no GitHub Pages

## Publicar no GitHub Pages

1. Crie um repositório no GitHub e envie estes arquivos para a branch `main`.
2. Abra **Settings → Pages**.
3. Em **Build and deployment**, selecione **Deploy from a branch**.
4. Escolha `main` e `/ (root)`, depois salve.

O site usa caminhos relativos e funciona tanto em `usuario.github.io/repositorio/` quanto em domínio próprio.

## YAML

Na abertura, o navegador busca `./tebasfin_cronograma_macro_padrao.yaml`. Em GitHub Pages esse arquivo é somente leitura no servidor. Alterações feitas no Gantt podem ser baixadas com **Baixar YAML**. Em Chrome/Edge, **Vincular YAML** permite escolher um arquivo YAML local e gravar nele automaticamente usando a File System Access API.

> Observação: GitHub Pages é hospedagem estática; alterações feitas no navegador não fazem commit no repositório. Para publicar um cronograma alterado, substitua o YAML no repositório e faça novo commit/push.
