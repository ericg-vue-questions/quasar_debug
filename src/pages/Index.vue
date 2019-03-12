<template>
  <q-page class="flex flex-center">
    <img alt="Quasar logo" src="~assets/quasar-logo-full.svg">

    <div v-for="value in returnArray()" :key="value.id">
      {{value}}<br />
    </div>
  </q-page>
</template>

<style>
</style>

<script>
export default {
  name: 'PageIndex',

  methods: {
    returnArray () {
      debugger
      console.log('in returnArray')
      return Array(5).fill().map((x, i) => i)
    }
  }
}
</script>
