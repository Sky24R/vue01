<template>
  <div class="source-code" v-highlightjs="txt">
    <pre><code class="javascript"></code></pre>
  </div>
</template>

<script>
import Vue from 'vue'
import VueHighlightJS from 'vue-highlightjs'
import 'highlight.js/styles/monokai-sublime.css'
Vue.use(VueHighlightJS)


export default {
  name: 'CodeHighlight',
  props: {
    txt: String
  }
}
</script>


<style lang="stylus" rel="stylesheet/stylus">
//@import '~highlight.js/styles/tomorrow.css';
code {
  margin-left: -0.5px !important;
  word-wrap: break-world !important;
  white-space: pre-wrap !important;
  max-height :30vh;
}

</style>
