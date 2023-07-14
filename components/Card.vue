<template>
  <div class="card py-3">
    <div class="top-section px-5">
      <div class="curs">$ 3 580</div>
      <div class="wrapper-question">
        <div class="question-icon">?</div>
      </div>
    </div>

    <div class="center-section px-5 mt-2">
      <div class="detail">Lorem ipsum dolor sit amet</div>
      <div class="curs-info">
        <p class="mt-5">+ 5,4% ($125)</p>
      </div>
    </div>

    <hr />

    <div class="bottom-section px-5">
      <div class="info-button mt-2">Lorem Ipsum</div>

      <div class="button-info">
        Lorem
        <span>
          <div class="wrapper-next">
            <font-awesome-icon
              icon="arrow-right"
              size="md"
              style="color: #ffffff; font-weight: bolder"
            />
          </div>
        </span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style>
.top-section,
.center-section,
.bottom-section {
  display: flex;
  justify-content: space-between;
}

.detail {
  width: 50%;
}
.card {
  border-radius: 20px;
  background: linear-gradient(
    313deg,
    #fbfbfb55 0%,
    rgba(178, 204, 255, 0.267) 80.64%
  );
  box-shadow: 3px 3px 7px 0px rgba(0, 0, 0, 0.25);
}
.curs {
  color: rgb(0, 0, 0);
  font-weight: 600;
  font-size: 25px;
}
.question-icon {
  width: 25px;
  height: 25px;
  border-radius: 100%;
  background-color: rgb(99, 0, 219);
  text-align: center;
  color: white;
  font-weight: bolder;
  font-size: 18px;
}
.detail {
  float: right;
  color: rgba(44, 44, 44, 0.688);
}
.curs-info {
  color: rgb(99, 0, 219);
  font-weight: bolder;
}
.info-button {
  color: rgba(29, 29, 29, 0.47);
  font-weight: bold;
  font-size: small;
}
.button-info {
  padding: 0.5em 2em;
  border-radius: 20px;
  color: white;
  font-weight: 600;
  background-color: rgb(255, 102, 252);
  box-shadow: 2px 2px 2px 0px rgb(162, 135, 166);
  display: flex;
  cursor: pointer;
  transition: 0.5s;
}
.button-info:hover {
  box-shadow: 4px 4px 4px 0px rgb(162, 135, 166);
  background-color: rgb(255, 80, 252);
}
.wrapper-next {
  margin-top: 2px;
  width: 23px;
  height: 23px;
  box-shadow: -2px -1px 2px 0px rgb(156, 96, 96);
  margin-left: 0.5em;
  border-radius: 100%;
  text-align: center;
  background-color: rgb(207, 89, 205);
}
</style>
