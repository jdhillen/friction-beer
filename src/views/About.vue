<!--|== Template =============================================================================== -->
<template>
  <MetaData :data="metaData" />
  <section>
    <div class="row">
      <div class="twelve columns">
        <h3>The Friction Story</h3>
      </div>
    </div>

    <div class="row">
      <div class="six columns">
        <img class="img" alt="" src="@/assets/img/pic01.jpg" />
      </div>
      <div class="six columns">
        <img class="img" alt="" src="@/assets/img/pic02.jpg" />
      </div>
    </div>

    <div class="row">
      <div class="twelve columns">
        <p>
          Around here we tend to say “timing is everything” a lot. Particularly in relation to how our
          founders Brent Anderson and Nathan Ryerson met and how Friction Beer Company came to be
          in the first place. You could say it was part fate, part serendipity, part patience (not always in
          big supply) and part bullheaded determination. But once that fire was lit, we had to keep it
          going.
        </p>
        <p>
          Flashback to 2011. Avid homebrewer and beer reviewer Nathan was already planning to fulfill a
          longtime dream of opening a brewery. But as often happens when cosmic forces aren’t aligned,
          life got in the way. He had the name and a larger idea of what he wanted it to be and still
          decided to put the project on a shelf until it made sense.
        </p>
        <p>
          Fast forward to fall of 2016. As he often did, Nathan was hosting a weekend soccer watch party.
          Equally fervent fan Brent showed up, having recently met Nathan at a brewery opening. Brent
          had recently left his marketing position as Creative Director for local beer legends Boulevard
          Brewing. Much beer was shared and discussed. And by the end of the match, the two hatched a
          plan to revive Nathan’s original plan. Only now, there was a team behind it.
        </p>
        <p>
          Many ups and downs followed that fortuitous morning. Countless potential spaces toured.
          Investors gained and lost. Successful pourings at beer fests. New friends and supporters made.
          Leases signed and plans scuttled. Lest we forget a freakin’ global pandemic. Through it all, the
          belief in the brand, the beer and all we had to offer never wavered.
        </p>
        <p>
          Which leads us to our fantastic first home in Shawnee, where apparently we were meant to be
          and why all that led up to our launch was entirely worth it. So here’s to social lubricants,
          healthy tension and Friction – from which comes the spark. To you and those who got us here,
          mighty thanks.
        </p>
      </div>
    </div>
  </section>
</template>

<!--|== Scripts ================================================================================ -->
<script>
import MetaData from '@/components/global/MetaData.vue';

export default {
  name: 'about-page',

  props: {},

  components: {
    MetaData
  },

  data() {
    return {
      metaData: {
        title: 'About',
        description: 'This is the description for the About page',
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
.about {
}

h1 {
  text-align: center;
}
</style>
