<!--|== Template =============================================================================== -->
<template>
  <footer class="footer">
    <div class="container">
      <div class="row">
        <div class="twelve columns footer__container">
          <div>Friction Beer Company - Copyright &copy; {{ useYear() }}</div>
          <div>
            <a href="https://goo.gl/maps/7EX6P79pJWhetuDP9" target="_blank">11018 Johnson Drive - Downtown Shawnee, KS</a>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<!--|== Scripts ================================================================================ -->
<script setup>
import { useYear } from '@/composables/useYear';
</script>

<!--|== CSS ==================================================================================== -->
<style lang="scss">
.footer {
  width: 100%;
  padding: 25px 0;
  font-family: 'Prohibition';
  color: $white;
  font-size: 14px;
  letter-spacing: 1px;
  text-align: center;

  &__container {
    display: flex;
    flex-direction: column-reverse;
    justify-content: space-between;

    @include breakpoint('sm') {
      flex-direction: row;
    }

    a {
      color: $white;
    }
  }
}
</style>
