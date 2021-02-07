<template>
  <section class="header">
    <div class="header-menu">
      <div class="logo">
        <nuxtLink to="/">
          <img src="~/assets/Logologo.png" alt="logo" />
        </nuxtLink>
      </div>
      <nav class="menu">
        <div class="menu__item">
          <nuxt-link to="/"> About </nuxt-link>
        </div>
        <div class="menu__item">
          <nuxt-link to="/"> Help </nuxt-link>
        </div>
        <div class="menu__item">
          <nuxt-link to="/"> Features </nuxt-link>
        </div>
        <div class="menu__item">
          <nuxt-link to="/"> Signup </nuxt-link>
        </div>
      </nav>
      <div class="request">
        <el-button class="request-btn btn"
          >Request Demo <i class="el-icon-right"></i
        ></el-button>
      </div>
    </div>
    <div class="main">
      <div class="main__content">
        <h1>Save your data storage here.</h1>
        <p>
          Data Warehouse is a data storage area that has been tested for
          security, so you can store your data here safely but not be afraid of
          being stolen by others.
        </p>
        <el-button class="btn btn-purple">Learn more</el-button>
      </div>
    </div>
    <div class="icon-storege"></div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scope>
// header

.header {
  width: 100%;

  position: relative;
}
.header-menu {
  width: 100%;
  display: flex;
  align-items: center;
  margin-top: 50px;
}
.logo {
  display: flex;
  align-items: center;
  justify-content: flex-start;
}
.menu {
  width: 100%;
  display: flex;
  margin-left: 50px;
  align-items: center;
  .menu__item {
    padding: 0px 15px;
  }
  a {
    color: #4b5d68;
    font-weight: 500;
    &:hover {
      color: #212353;
      font-weight: 800;
    }
  }
}
.request {
  width: 100%;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  .el-icon-right {
    color: #9c69e2;
  }
}
// main
.main {
  width: 100%;
  display: flex;
  flex-direction: column;
}
.main__content {
  margin-top: 130px;
  width: 50%;
  h1 {
    color: #212353;
    font-weight: bold;
    font-size: 80px;
    line-height: 110%;
  }
  p {
    margin-top: 50px;
    font-size: 18px;
    line-height: 160%;
    width: 55%;
  }
  .btn {
    margin-top: 50px;
  }
}
</style>
