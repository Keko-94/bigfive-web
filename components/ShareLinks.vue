<template>
  <div class="pt-5">
  </div>
</template>

<script>

export default {
  name: 'ShareLinks',
  props: {
    id: {
      type: String,
      default: ''
    }
  },
  data: () => ({
  }),
  methods: {
    logClick (type) {
      this.$amplitude.getInstance().logEvent('b5.sharing', { type })
    }
  }
}
</script>

<style scoped>
a {
  margin-right: 30px;
}
</style>
