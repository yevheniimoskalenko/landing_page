<template>
  <div>1</div>
</template>

<script>
export default {
  components: {},
  head() {
    return {
      title: 'Flycket',
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
