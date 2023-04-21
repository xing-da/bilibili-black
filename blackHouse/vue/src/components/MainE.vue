<template>
  <div class="main">
    <h3>{{ msg }}</h3>
  </div>
</template>

<script>
export default {
  name: "mainE",
  props: {
    msg: String,
  },
  beforeCreate(){},
  created(){},
};
</script>
<style scoped lang="scss"></style>
