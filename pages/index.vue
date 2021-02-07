<template>
  <div>
    <app-header />
    <app-features />
    <app-item-features />
    <app-testimonials />
    <app-footer />
  </div>
</template>

<script>
import appHeader from '~/components/header.vue';
import appFeatures from '~/components/features.vue';
import appItemFeatures from '~/components/itemFeatures.vue';
import appTestimonials from '~/components/testimonials.vue';
import appFooter from '~/components/footer.vue';
export default {
  components: {
    appHeader,
    appFeatures,
    appItemFeatures,
    appTestimonials,
    appFooter,
  },
  head() {
    return {
      title: '',
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {
          hid: 'description',
          name: 'description',
          content: 'My custom description',
        },

        {
          hid: 'keywords',
          name: 'keywords',
          content: 'Flycket',
        },
      ],
    };
  },
};
</script>
