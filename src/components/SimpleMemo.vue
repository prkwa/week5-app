// おしゃれヒューマンのapp
<template>
  <div class="container">
    <Human fashion="👚" />
    <Human fashion="👕" />
    <Human fashion="👔" />
  </div>
</template>

<script>
import Human from "@/components/Human.vue"

export default {
  components: {
    Human,
  },
}
</script>

<style scoped>
.container {
  display: flex;
}
</style>
