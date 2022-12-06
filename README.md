# dy-vite-vue-pdf
The package contains a [Vue2 + vite](https://vuejs.org/) component to easily display PDF files in Vite.

### Note: This project depends on [duyansoft-pdfjs-dist](https://github.com/yumeiqiang/duyansoft-pdfjs-dist) which is currently quite a few versions behind pdfjs-dist 

### Note: Make sure to manually copy [pdf.worker.min.js](https://cdn.jsdelivr.net/npm/pdfjs-dist@2.16.105/build/pdf.worker.min.js) to `public/pdsjs/pdf.worker.js`

## Example - basic
```vue
<template>
  <pdf src="./static/relativity.pdf"></pdf>
</template>

<script>
import pdf from 'dy-vite-vue-pdf'

export default {
  components: {
    pdf
  }
}
</script>
```
## 其他用法参考vue-pdf插件
## Install
```bash
yarn add --save dy-vite-vue-pdf
```

#### pdf.worker.js
Copy [pdf.worker.min.js](https://cdn.jsdelivr.net/npm/pdfjs-dist@2.16.105/build/pdf.worker.min.js) to `public/pdsjs/pdf.worker.js`. Vite-Vue3Pdf will load pdf.worker.js from https://cdn.jsdelivr.net/npm/pdfjs-dist@2.16.105/build/pdf.worker.min.js


## Demo

## Browser support
Same browser support as [Vue.js 3](https://github.com/vuejs/vue/blob/dev/README.md) (IE via Babel I guess)

## Note
- since v2.x, the script is exported as esm.
- This is a copy of [Vue-PDF](https://github.com/FranckFreiburger/vue-pdf#readme) adapted to work with Vue 3

## API