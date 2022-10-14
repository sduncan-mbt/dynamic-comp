<template>
  <div class="p-8">
    <template v-for="component in components" :key="component.id">
      <div class="mb-4">
        <component :is="component.name" :values="component"></component>
      </div>
    </template>
  </div>
</template>

<script>
import One from '~/components/One'
import Two from '~/components/Two'

export default {
  name: "Option",
  components: {
    One, Two
  },
  data() {
    return {
      components: [
        {id: 1, name: 'One', title: 'First is One'},
        {id: 2, name: 'Two', title: 'Second is Two'},
        {id: 3, name: 'One', title: 'Third is One'},
      ]
    }
  }
}
</script>