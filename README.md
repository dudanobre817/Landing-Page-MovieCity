 MovieCity
=========

> Uma vitrine de filmes no estilo streaming, feita para treinar React do zero.

MovieCity é uma landing page com fundo escuro, destaque em azul e uma grade de pôsteres. Ela nasceu como atividade do curso e serve de laboratório para três coisas: dividir a tela em componentes, escrever CSS sem ajuda de frameworks e fazer o layout funcionar bem tanto no computador quanto no celular.

<!-- Troque pelo caminho do seu print: -->
<!-- ![Tela inicial do MovieCity](./docs/preview.png) -->


## Em uma frase

Um cabeçalho com logo, links e botão de login, e logo abaixo o título **Seus Filmes** ao lado de seis pôsteres: Afterlife, Transformers, Mowgli, Shift, Round 6 e Harry Potter.


## Quer ver rodando?

Você precisa do [Node.js](https://nodejs.org) instalado (versão 20.19 ou superior).

```bash
git clone https://github.com/dudanobre817/Landing-Page-MovieCity.git
cd Landing-Page-MovieCity
npm install
npm run dev
```

Depois é só abrir `http://localhost:5173` no navegador.

Para gerar a versão final: `npm run build`. Para testá-la antes de publicar: `npm run preview`.


## Como o código está organizado

Pense na página como três blocos de montar:

- **Home** é a caixa grande que guarda tudo.
- **Header** é a faixa de cima (logo, menu e login).
- **Main** é a parte do meio (texto de chamada e pôsteres).

Os arquivos ficam assim:

```
src/
  components/   Header.jsx, Main.jsx e Home.jsx
  assets/       os pôsteres dos filmes
  App.jsx       chama o Home
  main.jsx      liga o React ao index.html
  index.css     todo o visual do projeto
```

O caminho que a página percorre até aparecer na tela:

`index.html` → `main.jsx` → `App.jsx` → `Home.jsx` → `Header.jsx` + `Main.jsx`


## Funciona no celular?

Funciona. A página muda conforme a largura da tela:

- **Telas grandes:** texto de um lado, pôsteres do outro, menu aberto no topo.
- **Telas médias:** as duas colunas passam a ficar uma sobre a outra.
- **Celulares:** os pôsteres se organizam em duas colunas e o menu vira um botão de hambúrguer.

Tudo isso é feito com `flexbox`, `grid` e `@media`, sem nenhuma biblioteca de componentes.


## Feito com

- React
- Vite
- CSS puro
- ESLint


## O que este projeto me ensinou

- Quebrar uma tela em componentes pequenos e reaproveitáveis.
- Importar imagens da pasta `src/assets` em vez de usar caminhos soltos.
- Usar `flexbox` e `grid` para posicionar elementos.
- Adaptar o layout para várias telas com media queries.
- Subir um projeto para o GitHub e organizar o repositório.


## Vontade de continuar

- [ ] Mostrar título e nota de cada filme nos cards
- [ ] Gerar os cards com `.map()` a partir de uma lista
- [ ] Buscar os filmes de uma API (como a TMDB)
- [ ] Publicar online com Vercel ou Netlify
- [ ] Fazer os pôsteres rolarem na horizontal no celular


## Autoria

Feito por [@dudanobre817](https://github.com/dudanobre817).
