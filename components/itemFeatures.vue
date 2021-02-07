<template>
  <section class="features__list">
    <div class="features__item green">
      <div class="features__container">
        <i class="icon-first"></i>
        <h3>Search Data</h3>
        <p>
          Don’t worry if your data is very large, the Data Warehoue provides a
          search engine, which is useful for making it easier to find data
          effectively saving time.
        </p>
        <nuxt-link to="/">Learn more <i class="el-icon-right"></i></nuxt-link>
      </div>
      <div class="features__image">
        <img src="~/assets/image3 1search.png" alt="search" />
      </div>
    </div>
    <div class="features__item purple">
      <div class="features__container">
        <i class="icon-second"></i>
        <h3>24 Hours Access</h3>
        <p>
          Access is given 24 hours a full morning to night and meet again in the
          morning, giving you comfort when you need data when urgent.
        </p>
        <nuxt-link to="/">Learn more <i class="el-icon-right"></i></nuxt-link>
      </div>
      <div class="features__image">
        <img src="~/assets/image4accesss.png" alt="access" />
      </div>
    </div>
    <div class="features__item pink">
      <div class="features__container">
        <i class="icon-three"></i>
        <h3>Print Out</h3>
        <p>
          Print out service gives you convenience if someday you need print
          data, just edit it all and just print it.
        </p>
        <nuxt-link to="/">Learn more <i class="el-icon-right"></i></nuxt-link>
      </div>
      <div class="features__image">
        <img src="~/assets/image5 1print.png" alt="access" />
      </div>
    </div>
    <div class="features__item blue">
      <div class="features__container">
        <i class="icon-four"></i>
        <h3>Security Code</h3>
        <p>
          Data Security is one of our best facilities. Allows for your files to
          be safer. The file can be secured with a code or password that you
          created, so only you can open the file.
        </p>
        <nuxt-link to="/">Learn more <i class="el-icon-right"></i></nuxt-link>
      </div>
      <div class="features__image">
        <img src="~/assets/image6 1.png" alt="access" />
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scope>
.features__list {
  display: flex;
  flex-wrap: wrap;
  flex-basis: 100%;
  justify-content: center;
  margin-top: 150px;

  .features__image {
    position: absolute;
    left: -150px;
    bottom: -10px;
    z-index: 3;
  }
  .features__image:nth-child(2) {
    position: absolute;
    bottom: -0px;
    left: -150px;
  }
  .features__item {
    position: relative;
    flex-basis: 32%;
    padding: 49px 50px;
    border-radius: 162px 60px 60px 60px;
    margin: 50px 100px;
    h3 {
      font-size: 24px;
      line-height: 32px;
      font-weight: normal;
    }
    p {
      margin-top: 20px;
    }
  }
}
.icon-first {
  position: absolute;
  width: 194px;
  height: 138px;
  background: url('~assets/item1.svg');
  background-size: cover;
  right: 30px;
  top: 10px;
  z-index: 2;
}
.icon-second {
  position: absolute;
  width: 251px;
  height: 252px;
  background: url('~assets/item2.svg');
  background-size: cover;
  right: 30px;
  bottom: -20px;
  z-index: 2;
}
.icon-three {
  position: absolute;
  width: 82px;
  height: 72px;
  background: url('~assets/item3.svg');
  background-size: cover;
  right: 20px;
  top: 10px;
  z-index: 2;
}
.icon-four {
  position: absolute;
  width: 364px;
  height: 268px;
  background: url('~assets/item4.svg');
  background-size: cover;
  right: 140px;
  top: 0px;
  z-index: 2;
}
.features__container {
  width: 80%;
  margin-left: 90px;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: space-between;
  z-index: 3;
  a {
    margin-top: 20px;
    z-index: 3;
  }
}

.green {
  background: rgba(#68c9ba, 0.1);
}
.purple {
  background: rgba(#9c69e2, 0.1);
}
.pink {
  background: rgba(#f063b8, 0.1);
}
.blue {
  background: rgba(#2d9cdb, 0.1);
}
</style>
