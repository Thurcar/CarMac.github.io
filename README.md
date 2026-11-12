# Portfólio: Arthur Carneiro Maciel

Site estático (HTML, CSS e JavaScript puro), pronto para o GitHub Pages. Não precisa de build nem de npm.

## Estrutura
- `index.html`: esqueleto da página
- `js/content.js`: **todo o conteúdo** (é o único arquivo que você precisa editar)
- `js/app.js` e `css/style.css`: montagem e visual
- `assets/images`, `assets/gifs`, `assets/videos`: suas mídias

## O que trocar primeiro
1. Coloque sua foto em `assets/images/foto.jpg` (sem ela, o site mostra suas iniciais).
2. Em `content.js`, troque os links de LinkedIn e Gmail na seção `contato`.
3. Ajuste os textos de "Sobre mim", dos projetos e das datas da educação.

## Adicionar mídia a um projeto
Dentro do projeto, preencha `midia` (a primeira vira a capa do card):
```js
midia: [
  { tipo: "gif",     src: "assets/gifs/gameplay.gif", legenda: "Gameplay" },
  { tipo: "imagem",  src: "assets/images/menu.png" },
  { tipo: "video",   src: "assets/videos/demo.mp4" },
  { tipo: "youtube", id: "ID_DO_VIDEO" }
]
```
Para vídeos longos, prefira `youtube`. O GitHub aceita arquivos de até 100 MB.

## Criar novas seções
Copie um bloco de `secoes` e escolha o `tipo`: `projetos`, `habilidades`, `educacao`, `texto`, `galeria` ou `contato`.
A ordem do array é a ordem na página, e o menu é gerado sozinho (use `menu: false` para esconder um item).

## Publicar no GitHub Pages
1. Crie um repositório no GitHub (ex.: `portfolio`, ou `seu-usuario.github.io` para URL curta).
2. Envie todos os arquivos desta pasta para ele.
3. Vá em **Settings → Pages → Build and deployment → Deploy from a branch**, escolha `main` e `/ (root)` e salve.
4. Em alguns minutos o site fica em `https://seu-usuario.github.io/portfolio/`.

Para testar localmente, abra o `index.html` no navegador ou use a extensão Live Server do VS Code.
