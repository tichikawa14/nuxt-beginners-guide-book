<template>
  <div>
    <p>{{ toggleStatus }}</p>
    <button type="button" @click="toggle">toggle</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      status: false
    }
  },
  methods: {
    toggle() {
      this.status = !this.status
    }
  },
  computed: {
    toggleStatus() {
      return status ? 'on' : 'off'
    }
  }
}
</script>
