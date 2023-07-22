# vuejs

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Compile and Minify for Production

```sh
npm run build

```
Vamos configurar nosso setup:
Para começar vamos apagar as pastas em src:
    assets
    components

Em App.vue vamos remover essas duas referencias:

No <script> exclui:

    import HelloWorld from './components/HelloWorld.vue'
    import TheWelcome from './components/TheWelcome.vue'

No <template> exclui tudo e cria um h1 com Hello Word.

Em <style> só deixamos as tags.

Em main.js vamos remover essas referencias:

    a referenciade css

____________________________________________________________________________

v-if
v-show
v-else-if
tomar cuidado com a posição das tags a cima 





