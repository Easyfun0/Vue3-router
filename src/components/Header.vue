<template>
  <div class="container">
    <button @click.prevent="goForm" class="btn">開啟</button>
    <!-- <router-view /> -->
  </div>
</template>  

<script>
export default {
  name: "Header",
  props: {
    msg: String,
  },
  methods: {
    goForm() {
      this.$router.push("/form");
    },
  },
};
</script>