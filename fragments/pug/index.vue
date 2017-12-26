<template lang='pug'>
{{#if module}}
  div(:class="$style['{{kebab __NAME__}}']")
{{else}}
  .{{kebab __NAME__}}
{{/if}}
</template>

<script>
  export default {
    name: '{{__NAME__}}'
  }
</script>

{{#if style}}
<style lang='{{style}}' {{{couple module 'module'}}}{{{couple scoped 'scoped'}}}>
  {{>(partial style)}}
</style>
{{else}}
<style {{{couple module 'module'}}}{{{couple scoped 'scoped'}}}>
  {{>css}}
</style>
{{/if}}
