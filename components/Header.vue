<template>
  <header class="header">
    <nav class="navbar px-5" role="navigation" aria-label="main navigation">
      <div id="navbarBasicExample" class="navbar-menu">
        <div class="navbar-start">
          <div class="navbar-item">
            <span class="tag py-5 px-6 is-active-tag">
              <p>Lorem ipsum</p>
            </span>
          </div>

          <div class="navbar-item">
            <span class="tag py-5 px-6">
              <p>Lorem ipsum</p>
            </span>
          </div>

          <div class="navbar-item">
            <span class="tag py-5 px-6">
              <p>Lorem ipsum</p>
            </span>
          </div>
        </div>

        <div class="navbar-end wrapper-navbar-end">
          <div class="navbar-item item">
            <div class="buttons">
              <a class="is-primary">
                <span class="icon-text">
                  <span class="icon">
                    <font-awesome-icon
                      icon="magnifying-glass"
                      size="2xl"
                      style="color: #9589d1"
                    />
                  </span>
                </span>
              </a>
            </div>
          </div>

          <div class="navbar-item item">
            <div class="buttons">
              <a class="is-primary">
                <span class="icon-text">
                  <span class="icon">
                    <font-awesome-icon
                      icon="bell"
                      style="color: #9589d1"
                      size="2xl"
                    />
                  </span>
                </span>
              </a>
            </div>
          </div>

          <div class="navbar-item item">
            <div class="buttons">
              <a class="is-primary">
                <span class="icon-text">
                  <span class="icon">
                    <font-awesome-icon
                      icon="user"
                      size="2xl"
                      style="color: #9589d1"
                    />
                  </span>
                </span>
              </a>
            </div>
          </div>
        </div>
      </div>
    </nav>
  </header>
</template>

<script>
export default {};
</script>

<style>
header {
  border-radius: 35px 35px 0 0;
  box-shadow: 0px 15px 30px 0px rgba(0, 0, 0, 0.17);
  height: 90px;
  background-color: #e3f2ff;
}
.navbar {
  background: transparent;
  height: 90px;
}
.wrapper-chip {
  margin-left: 22em;
}
.wrapper-chip div {
  float: left;
}
.chip {
  margin-right: 2em;
  line-height: 80px;
}

.tag {
  border-radius: 50px !important;
  background: rgb(255, 255, 255);
  font-size: 13px !important;
}
.is-active-tag {
  background-color: rgb(59, 255, 173) !important;
  color: white !important;
  font-weight: 600;
}
.wrapper-navbar-end .item {
  margin-left: 5em;
}
</style>
