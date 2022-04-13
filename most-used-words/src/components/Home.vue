<template>
<div class="pills">
  <Pill v-for="word in groupdWords" :key="word.name"
  :name="word.name" :amount="word.amount"
  />
</div>
</template>

<script>
import Pill from "./Pill";
export default {
  name: "HomeInit",
  components: {
    Pill
  },
  data: () => ({
    groupdWords: [
      {name: 'i', amount:123},
      {name: 'you', amount:1223},
      {name: 'he', amount:333},
    ]
  }),
}
</script>

<style scoped>

</style>