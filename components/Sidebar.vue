<template>
  <aside class="sidebar py-6">
    <nav>
      <a href="#" class="wrapper-logo">
        <div class="logo-img">L</div>
        <div class="logo"><p class="mt-1">LOGO</p></div>
      </a>
      <div class="title-sidebar">
        <p>Lorem</p>
      </div>

      <div class="wrapper-list-sidebar">
        <ul>
          <li class="active">
            <font-awesome-icon
              class="icon-list"
              icon="house"
              style="color: #513f92"
              size="xl"
            />
            Lorem ipsum
          </li>
          <li>
            <font-awesome-icon
              class="icon-list"
              icon="shield"
              style="color: #513f92"
              size="xl"
            />
            Dolor Sit
          </li>
          <li>
            <font-awesome-icon
              icon="lock"
              class="icon-list"
              style="color: #513f92"
              size="xl"
            />
            Amet Consectetur
          </li>
          <li>
            <font-awesome-icon
              icon="dollar-sign"
              class="icon-list"
              style="color: #513f92"
              size="xl"
            />
            Accusantium Neque
          </li>
          <li>
            <font-awesome-icon
              icon="gear"
              class="icon-list"
              style="color: #513f92"
              size="xl"
            />
            Adipisicing Elit
          </li>
        </ul>
      </div>

      <div class="wrapper-box-premium">
        <div class="box-premium">
          <p class="title-premium">LOREM IPSUM</p>
          <p class="body-premium">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit
            totam, dolor
          </p>
          <div class="wrapper-button-premium">
            <div class="button-premium">LOREM</div>
          </div>
        </div>
      </div>
    </nav>
  </aside>
</template>

<script lang="ts">
export default {};
</script>

<style scoped>
.sidebar {
  margin: 0;
  float: left;
  border-radius: 35px;
  background: #7e4dfd;
  height: 650px;
  overflow-x: hidden;
  overflow-y: scroll;
  width: 350px;
  transition: 0.5s;
}
.logo-img {
  border-radius: 100%;
  background: rgba(255, 135, 135, 0.75);
  box-shadow: 5px 5px 20px 2px rgba(102, 57, 57, 0.49);
  color: white;
  font-weight: bold;
  font-size: 45px;
  height: 65px;
  width: 65px;
  text-align: center;
}
.logo {
  border: 3px solid rgb(255, 166, 0);
  border-radius: 10px;
  font-size: 32px;
  font-weight: 500;
  color: white;
  width: max-content;
  padding: 0 0.5em;
  margin-left: 0.5em;
  text-align: center;
  align-items: center;
}
.wrapper-logo {
  display: flex;
  justify-content: center;
  margin-left: -3em;
}
.title-sidebar p {
  margin-left: 3em;
  margin-top: 3em;
  color: white;
  font-size: larger;
  font-weight: 600;
}
.wrapper-list-sidebar {
  margin-left: 2.8em;
}
.wrapper-list-sidebar li {
  margin: 1em 0;
  font-size: medium;
  color: white;
  padding: 1em 0 1em 1em;
  border-radius: 30px 0px 0px 30px;
  cursor: pointer;
}
.active {
  background-color: #5c2cd8 !important;
}
.icon-list {
  margin-right: 0.75em;
}
.wrapper-box-premium {
  display: flex;
  justify-content: center;
  margin-top: 3em;
}
.box-premium {
  fill: linear-gradient(
    315deg,
    #8258f1 0%,
    rgba(130, 86, 243, 0.82) 30.21%,
    rgba(71, 0, 255, 0) 100%
  );
  box-shadow: 25px 25px 30px 0px rgba(0, 0, 0, 0.2) inset,
    5px 6px 10px 0px #18181853;
  filter: drop-shadow(5px 10px 25px rgba(255, 255, 255, 0.25));
  width: 260px;
  border-radius: 20px;
  padding: 1em;
  color: white;
}
.body-premium {
  color: #3e3e3e;
  font-size: 13px;
  margin-top: 0.5em;
}
.wrapper-button-premium {
  display: flex;
  justify-content: center;
}
.button-premium {
  background-color: rgb(255, 217, 0);
  padding: 0.5em 2em;
  border-radius: 25px;
  color: black;
  font-weight: 550;
  box-shadow: 3px 3px 10px 0px white;
  margin-top: 1em;
  cursor: pointer;
  transition: 0.5s;
}
.button-premium:hover {
  box-shadow: 4px 4px 20px 0px white;
  background-color: rgb(255, 242, 0);
}
</style>
