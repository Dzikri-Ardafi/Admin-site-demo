<template>
  <div class="box">
    <NuxtPage />
  </div>
</template>

<style>
@import "bulma/css/bulma.css";
@import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,400;0,700;0,900;1,400;1,700;1,900&display=swap");
* {
  padding: 0;
  margin: 0;
}
body {
  background-color: #9c83f9;
  font-family: "Poppins", sans-serif;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.box {
  padding: 0;
  margin: 0;
  border-radius: 35px;
  background: #dde9ff;
  box-shadow: 20px 20px 30px 0px rgba(0, 0, 0, 0.17);
  width: 1400px;
  height: 650px;
}
::-webkit-scrollbar {
  width: 0px;
}

::-webkit-scrollbar-track {
  background-color: transparent;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: #2600be00;
  border-radius: 10px;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #2600be00;
}
</style>
