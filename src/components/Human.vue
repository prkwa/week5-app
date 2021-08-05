<template>
  <div class="human">
    <div class="atama">
      <div v-if="isLaughing">🤣</div>
      <div v-else>😊</div>
    </div>
    <div class="karada" v-on:click="makeLaugh">
      <div>💪{{ fashion }}💪</div>
    </div>
    <div class="ashi">
      <div>🦵🦵</div>
    </div>
  </div>
</template>

<style>
.human {
  width: 10rem;
  font-size: 3rem;
  text-align: center;
}
</style>
<script>
export default {
  props: ["fashion"],
  data() {
    return {
      isLaughing: false,
    }
  },
  methods: {
    makeLaugh() {
      this.isLaughing = true
    },
  },
}
</script>
