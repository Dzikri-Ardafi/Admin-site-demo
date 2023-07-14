<template>
  <div class="container content px-6 py-5 pb-5">
    <div class="wrapper-column-1">
      <div class="mb-5 chart-2">
        <ChartChart2 />
      </div>

      <div class="mb-5 dropdowm">
        <Dropdown />
      </div>
    </div>

    <div class="wrapper-column-2">
      <div class="mb-5 chart-3">
        <ChartChart3 />
      </div>

      <div class="mb-5 card">
        <Card />
      </div>
    </div>

    <div class="wrapper-column-3">
      <div class="mb-5">
        <ChartChart4 />
      </div>
      <div class="mb-5 chart-1">
        <ChartChart1 />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.content {
  display: flex;
  max-height: 560px;
  max-width: 1400px;
  overflow-x: auto;
  overflow-y: scroll;
}
.wrapper-column-2 {
  margin: 0 4em;
}
</style>
