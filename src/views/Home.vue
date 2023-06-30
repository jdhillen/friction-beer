<!--|== Template =============================================================================== -->
<template>
  <MetaData :data="metaData" />
  <section class="home">
    <hr>
    <div class="row">
      <div class="twelve columns">
        <h5>A New Website is Coming Soon!</h5>
      </div>
    </div>
    <hr>
    <div class="row">
      <div class="twelve columns">
        <img class="img" alt="" src="@/assets/img/building.png" />
      </div>
    </div>
    <hr>
    <div class="row">
      <div class="six columns">
        <h3>Hours</h3>
        <ul>
          <li><strong>Thursday</strong>: 4pm - 10pm</li>
          <li><strong>Friday</strong>: 4pm - 10pm</li>
          <li><strong>Saturday</strong>: 12pm - 10pm</li>
          <li><strong>Sunday</strong>: 12pm - 7pm</li>
        </ul>
      </div>
      <div class="six columns">
        <h3>Directions</h3>
        <a href="https://goo.gl/maps/vq3EUog1hr7N5xY86" target="_blank" rel="noopener noreferrer">11018 Johnson Dr<br/>Shawnee, KS 66203</a>
      </div>
    </div>
    <hr>
    <div class="row">
      <div class="twelve columns">
        <footer>Copyright © 2023 - Friction Brewing Company</footer>
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
        description: 'A music soaked beer experience featuring an ever-evolving array of fantastically-flavorful, hoppy, stouty beers.',
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

  ul {
    list-style-type: none;
    padding: 0;
    margin: 0;
  }

  footer {
    font-size: 12px;
    margin-bottom: 50px;
  }
}
</style>
