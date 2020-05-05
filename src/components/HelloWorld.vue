<template>
  <div class="board">
      <div class="mancala"></div>
      <div v-for="n in 10" class="pit" :key="n">{{ n }}</div>
      <div class="mancala"></div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class HelloWorld extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.mancala {
  border: 2px;
}
.pit {
  border: 2px;
}
</style>
