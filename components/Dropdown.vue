<template>
  <div class="dropdown-1 mb-5">
    <font-awesome-icon
      class="mr-5"
      icon="chart-simple"
      style="color: #513f92"
      size="xl"
    />

    <span class="title-dropdown">LOREM IPSUM</span>

    <div class="wrapper-icon-dropdown">
      <font-awesome-icon
        class="mt-2"
        icon="chevron-down"
        size="xl"
        style="color: #000000"
      />
    </div>
  </div>

  <div class="dropdown-1">
    <font-awesome-icon
      class="mr-5"
      icon="database"
      style="color: #513f92"
      size="xl"
    />

    <span class="title-dropdown">Dolor Sit Amet</span>

    <div class="wrapper-icon-dropdown">
      <font-awesome-icon
        class="mt-2"
        icon="chevron-down"
        size="xl"
        style="color: #000000"
      />
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style>
.dropdown-1 {
  width: 100%;
  border-radius: 20px;
  background: linear-gradient(
    313deg,
    #e4f5ff 0%,
    rgba(136, 175, 255, 0.75) 80.64%
  );
  box-shadow: 7px 7px 10px 0px rgba(0, 0, 0, 0.25);
  padding: 0.5em;
  padding: 1em;
  border-radius: 20px;
}
.title-dropdown {
  color: rgb(94, 94, 94);
  font-weight: 600;
}
.wrapper-icon-dropdown {
  display: flex;
  justify-content: center;
  width: 40px;
  height: 40px;
  border-radius: 100%;
  background-color: rgb(255, 132, 0);
  float: right;
  margin-top: -0.3em !important;
}
</style>
