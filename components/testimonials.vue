<template>
  <section class="testimonials">
    <div class="testimonials__main">
      <h2>Testimonials</h2>
      <el-carousel :interval="4000" type="card">
        <el-carousel-item v-for="(review, index) in reviews" :key="index">
          <div class="reviews__item">
            <div class="review__photo">
              <img
                :src="require(`~/assets/img/${review.photo}.png`)"
                :alt="review.name"
              />
            </div>
            <div class="review__info">
              <h4>{{ review.name }}</h4>
              <span>{{ review.sub }}</span>
              <p>{{ review.message }}</p>
            </div>
          </div>
        </el-carousel-item>
      </el-carousel>
    </div>
  </section>
</template>
<script>
export default {
  data() {
    return {
      reviews: [
        {
          name: 'John Fang',
          sub: 'wordfaang.com',
          photo: 'user1',
          message:
            'Suspendisse ultrices at diam lectus nullam. Nisl, sagittis viverra enim erat tortor ultricies massa turpis. Arcu pulvinar aenean nam laoreet nulla.',
        },
        {
          name: 'Jeny Doe',
          sub: 'UX Engineer',
          photo: 'user2',
          message:
            'Suspendisse ultrices at diam lectus nullam. Nisl, sagittis viverra enim erat tortor',
        },
        {
          name: 'John Fang',
          sub: 'Web Designer',
          photo: 'user3',
          message:
            'Suspendisse ultrices at diam lectus nullam. Nisl, sagittis viverra enim erat tortor',
        },
      ],
    };
  },
  components: {},
};
</script>
<style lang="scss" scope>
.testimonials {
  margin-top: 150px;
}
.testimonials__main {
  background: #9c69e2;
  border-radius: 50px;
  padding: 109px 93px;
  h2 {
    color: #fff;
    font-weight: bold;
    font-size: 40px;
    margin-bottom: 88px;
  }
}

.reviews__item {
  height: 330px;
  display: flex;
  flex-direction: row;
  .review__photo {
    height: 100%;
    display: flex;
    flex-direction: column;
    margin-right: 30px;
  }
  .review__info {
    display: flex;
    flex-direction: column;
    height: 100%;
    h4 {
      color: #212353;
    }
    span {
      color: #9c69e2;
      font-size: 14px;
    }
    p {
      margin-top: 20px;
      font-size: 18px;
      line-height: 32px;
    }
  }
}
</style>
