<template>
  <section class="features">
    <div class="features__wrapper">
      <div class="features__main">
        <div class="featur">
          <img src="~/assets/image2features.png" alt="features" />
        </div>
        <div class="features__contain">
          <h2>We are a high-level data storage bank</h2>
          <p>
            The place to store various data that you can access at any time
            through the internet and where you can carry it. This very flexible
            storage area has a high level of security. To enter into your own
            data you must enter the password that you created when you
            registered in this Data Warehouse.
          </p>
        </div>
      </div>
      <span>Features</span>
    </div>
    <p class="features__bottom">
      Some of the features and advantages that we provide for those of you who
      <br />
      store data in this Data Warehouse.
    </p>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scope>
.features {
  width: 100%;
  position: relative;
  flex-direction: column;
  display: flex;
  height: 100%;
  margin-top: 268px;
}
.features__bottom {
  margin-top: 20px;
  text-align: center;
}
.features__wrapper {
  display: flex;
  flex-direction: column;
  background: rgba(240, 99, 184, 0.15);
  width: 100%;
  border-radius: 50px;
  padding: 40px 50px;
  span {
    text-align: center;
    font-weight: bold;
    font-size: 40px;
  }
}
.features__main {
  display: flex;
  padding: 30px 50px;
  align-items: center;
}
.featur {
  flex-basis: 50%;
}
.features__contain {
  flex-basis: 50%;
  h2 {
    font-size: 40px;
    font-weight: bold;
    line-height: 52px;
  }
  p {
    margin-top: 30px;
  }
}
</style>
