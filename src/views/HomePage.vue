<!--|== Template =============================================================================== -->
<template>
  <section class="home container">
    <div class="row">
      <div class="twelve columns">
        <img alt="Friction Brewing Company Badge" src="@/assets/img/badge.png" class="badge" />
      </div>
    </div>
    <div class="row">
      <div class="twelve columns times">
        <div class="times__header">Now Open.</div>
        <div class="times__day">Thursday&emsp;4pm - 10pm</div>
        <div class="times__day">Friday&emsp;4pm - 10pm</div>
        <div class="times__day">Saturday&emsp;12am - 10pm</div>
        <div class="times__day">Sunday&emsp;12am - 7pm</div>
      </div>
    </div>

    <div class="row">
      <div class="twelve columns">
        <form name="Mailing List" class="mailing-form" data-netlify="true">
          <label>
            <input type='email' name="email" placeholder="Enter Your Email For News and updates." pattern="[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,4}$" />
          </label>
          <button type="submit" class="mailing-form__button">Submit</button>
        </form>
      </div>
    </div>

    <div class="row">
      <div class="twelve columns social">
        <div class="social__logo">
          <img alt="Friction Brewing Company Logo" src="@/assets/img/logo.png"/>
        </div>
        <div class="social__icons">
          <ul>
            <li>
              <a 
                href="https://www.facebook.com/FrictionBeer/"  
                target="_blank"
                alt="Facebook | Friction Brewing Company"
                aria-label="Facebook"
                class="icon icon__social icon__facebook"
              >
              </a>
            </li>
            <li>
              <a 
                href="https://www.instagram.com/frictionbeer/"  
                target="_blank"
                alt="Instagram | Friction Brewing Company"
                aria-label="Instagram"
                class="icon icon__social icon__instagram"
              >
              </a>
            </li>
            <li>
              <a 
                href="https://twitter.com/frictionbeer/"  
                target="_blank"
                alt="Twitter | Friction Brewing Company"
                aria-label="Twitter"
                class="icon icon__social icon__twitter"
              >
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<!--|== Scripts ================================================================================ -->
<script setup>
</script>

<!--|== CSS ==================================================================================== -->
<style lang="scss" scoped>
.home {
  text-align: center;

  @include breakpoint('sm') {
    text-align: left;
  }
}

.badge {
  height: auto;
  width: 100%;
  max-width: 150px;
  margin-top: 85px;

  @include breakpoint('sm') {
    max-width: 275px;
    margin-top: 50px;
  }
}

.times {
  font-family: 'Prohibition';
  color: $white;
  text-align: right;
  margin-top: 150px;
  text-align: center;

  @include breakpoint('sm') {
    margin-top: 25px;
    text-align: right;
  }

  &__header {
    font-size: 35px;

    @include breakpoint('sm') {
      font-size: 50px;
    }
  }

  &__day {
    font-size: 20px;
    line-height: 30px;
    

    @include breakpoint('sm') {
      font-size: 35px;
      line-height: 45px;
    }
  }
}

.social {
  display: flex;
  flex-direction: column;
  justify-content: space-between;

  @include breakpoint('sm') {
    flex-direction: row;
    justify-content: space-between;
  }

  &__logo {
    img {
      width: 150px;

      @include breakpoint('sm') {
        width: 240px;
      }
    }
  }

  &__icons {
    display: flex;
    flex-direction: row;
    justify-content: center;

    ul {
      margin: 0 auto;
      padding: 0;
      list-style-type: none;
      display: flex;
      flex-direction: row;
      flex-wrap: wrap;
      align-items: center;
      justify-content: center;

      li {
        display: flex;
        margin: 10px;

        a {
          color: white(0.75);
          transition: 300ms color;

          &:hover {
            color: $white;
          }
        }
      }
    }
  }
}

.mailing-form {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 50px;
  
  @include breakpoint('sm') {
    flex-direction: row;
    align-items: initial;
  }

  label {
    width: 100%;
  }
  
  input[type='email'] {
    width: 100%;
    border-radius: 0;
    padding: 25px;
    text-align: center;
  }

  &__button {
    background-color: $gray;
    border-radius: 0;
    height: 52px;
    width: 175px;
    font-family: 'Prohibition';
    letter-spacing: 5px;
    font-size: 18px;
    color: $black;
  }

  ::placeholder {
    color: black(0.75);
    font-family: 'Prohibition';
    font-size: 12px;
    letter-spacing: 1px;
    text-align: center;
  }
}
</style>