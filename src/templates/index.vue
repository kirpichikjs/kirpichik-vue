<template>
  <div class="{{ __NAME__ | kebab }}">

  </div>
</template>

<script>
  export default {
    name: '{{ __NAME__ }}',

    data() {
      return {

      }
    }
  }
</script>

<style>
  .{{ __NAME__ | kebab }} {
    display: block;
  }
</style>
