<template>
  <div id="app"></div>
</template>

<script>
export default {
  async created() {
    await this.$store.dispatch("changeDataAction1");
    await this.$store.dispatch("changeDataAction2");
    console.log(this.$store.state.data1.data);
    console.log(this.$store.state.data2.data);
  },
};
</script>
