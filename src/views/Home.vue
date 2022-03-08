<!--|== Template =============================================================================== -->
<template>
  <MetaData :data="metaData" />
  <section class="home">
    <h1>Coming Soon!</h1>
    <div class="row">
      <div class="twelve columns">
        <img class="img" alt="" src="@/assets/img/building.jpg" />
      </div>
    </div>
  </section>
</template>

<!--|== Scripts ================================================================================ -->
<script>
import MetaData from '@/components/global/MetaData.vue';

export default {
  name: 'home-page',

  props: {},

  components: {
    MetaData,
  },

  data() {
    return {
      metaData: {
        title: 'Home',
        description: 'This is the description for the Home page',
        image: 'https://via.placeholder.com/1500x780'
      }
    };
  },

  beforeCreate() {},

  created() {},

  beforeMount() {},

  mounted() {},

  beforeUpdate() {},

  updated() {},

  beforeUnmount() {},

  unmounted() {},

  computed: {},

  methods: {},

  watch: {}
};
</script>

<!--|== CSS ==================================================================================== -->
<style lang="scss" scoped>
.home {
  text-align: center;
}
</style>
