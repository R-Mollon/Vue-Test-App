<template>
  <div>{{ title }}</div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: ['title'],
  data() {
      return {
          height: '80px',
          backgroundColor: '#0099cc',
      }
  }
}
</script>

<style scoped>
    div {
        width: 100vw;
        min-width: fit-content;
        height: v-bind(height);

        background: v-bind(backgroundColor);

        display: block;
        position: absolute;
        left: 0;
        top: 0;

        font-size: 3em;
        line-height: v-bind(height);

        white-space: nowrap;
    }
</style>
