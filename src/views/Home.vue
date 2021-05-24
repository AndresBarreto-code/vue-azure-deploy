<template>
  <div class="home">
    <h2>{{ title }}</h2>
  </div>
</template>

<script>
export default {
  name: 'Home',
  props: {
    title: {
      type: String,
      required: true
    }
  },
  data() {
    return {

    }
  }
}
</script>
