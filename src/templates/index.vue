{{#if pug}}
<template lang="pug">
  .{{kebab __NAME__}}
</template>
{{else}}
<template>
  <div class="{{kebab __NAME__}}">

  </div>
</template>
{{/if}}

<script>
  export default {
    name: '{{__NAME__}}',

    data() {
      return {

      }
    }
  }
</script>

{{#if styl}}
<style lang="stylus">
  .{{kebab __NAME__}}
    display block
</style>
{{else}}
<style>
  .{{kebab __NAME__}} {
    display: block;
  }
</style>
{{/if}}
