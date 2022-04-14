<template>
  <v-container fluid>
    <div class="pills">
      <Pill v-for="word in groupdWords" :key="word.name"
            :name="word.name" :amount="word.amount"
      />
    </div>
  </v-container>
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
      {name: 'i', amount: 123},
      {name: 'you', amount: 1223},
      {name: 'he', amount: 333},
      {name: 'i', amount: 123},
      {name: 'you', amount: 1223},
      {name: 'he', amount: 333},
      {name: 'i', amount: 123},
      {name: 'you', amount: 1223},
      {name: 'he', amount: 333},
      {name: 'i', amount: 123},
      {name: 'you', amount: 1223},
      {name: 'he', amount: 333},
      {name: 'he', amount: 333},
      {name: 'he', amount: 333},
      {name: 'he', amount: 333},
      {name: 'he', amount: 333},
      {name: 'he', amount: 333},
      {name: 'he', amount: 333},
      {name: 'he', amount: 333},
      {name: 'he', amount: 333},
      {name: 'he', amount: 333},
      {name: 'he', amount: 333},
    ]
  }),
}
</script>

<style scoped>
.pills {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
</style>