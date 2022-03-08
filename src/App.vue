<!--|== Template =============================================================================== -->
<template>
  <section class="app container">
    <div class="row align">
      <div class="four columns">
        <img class="logo" alt="Vue logo" src="@/assets/img/logo.png" />
      </div>
    </div>
    <div class="row">
      <div class="twelve columns">
        <div id="nav" class="nav">
          <router-link :to="{ name: 'Home' }">Home</router-link>
          <span>&nbsp;&nbsp;|&nbsp;&nbsp;</span>
          <router-link :to="{ name: 'About' }">About</router-link>
        </div>
      </div>
    </div>
    <router-view />
  </section>
</template>

<!--|== Scripts ================================================================================ -->
<script>
export default {
  name: 'app',

  props: {},

  components: {},

  data() {
    return {};
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
<style lang="scss">
.app {
  margin-top: 50px;
}

.nav {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  margin-bottom: 50px;
}

.align {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

.logo {
  width: 100%;
  height: auto;
  margin-bottom: 50px;
}
</style>
