<template>
  <div>
    <Sidebar />
  </div>

  <div>
    <Header />
  </div>

  <div>
    <Content />
  </div>
</template>

<script lang="ts">
export default {
  data() {
    return {
      title: "This is s",
    };
  },
  mounted() {
    console.log(this.title);
  },
};
</script>

<style scoped></style>
