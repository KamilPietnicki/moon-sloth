<template>
  <div class="landing">
    <div class="landing-wrap">
      <div class="landing-logo">
        <img src="~/assets/sloth-main.png" />
      </div>
      <div class="landing-text">
        <!-- <h1 class="title">MOON SLOTH 🦥🌙</h1> -->
        <h1 class="title">MOON SLOTH</h1>
        <h2 class="subtitle">
          $MoonSloth is a community-focused, decentralized cryptocurrency with instant rewards for holders.
        </h2>
        <div class="links">
          <h3 class="h3">Join our mission</h3>
          <a
            href="https://vuesax.com/"
            target="_blank"
            rel="noopener noreferrer"
            class="button--grey"
          >
            Telegram
          </a>
          <a
            href="https://discordapp.com/invite/9dsKtvB"
            target="_blank"
            rel="noopener noreferrer"
            class="button--grey"
          >
            Twitter
          </a>
        </div>
      </div>
    </div>

    <div class="arrow">
      <div class="arrow-top"></div>
      <div class="arrow-bottom"></div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
};
</script>

<style lang="scss">
.landing {
  display: block;
  position: relative;
  width: 100%;
  height: 100vh;
}

.landing-wrap {
  display: grid;
  position: absolute;

  width: calc(100% - 160px);
  max-width: 740px;
  height: auto;

  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);

  grid-template-columns: auto 1fr;
  column-gap: 80px;
  align-items: center;

  @media (min-width: 992px){
    width: calc(100% - 80px);
  	column-gap: 80px;
  }

  @media (max-width: 767.98px){
  	display: block;
    width: 100%;

    .landing-logo {
      display: block;
      position: absolute;

      top: 50%;
      left: 50%;

      transform: translate(-50%, -50%);

      z-index: 0;

      img {
        opacity: 0.25;
      }
    }

    .landing-text {
      display: block;
      position: absolute;

      width: calc(100% - 40px);
      height: auto;

      top: 50%;
      left: 50%;

      transform: translate(-50%, -50%);

    }
  }

  h3 {
    margin-bottom: 10px;
  }
}

.arrow {
  cursor: pointer;
  height: 120px;
  left: 50%;
  position: absolute;
  bottom: 80px;
  transition: transform .1s;
  width: 80px;
  transform: rotate(90deg) translate(-50%, 0%);
  
  $transition-time: .15s;
  
  &-top,
  &-bottom {
    background-color: #666;
    height: 4px;
    left: -5px;
    position: absolute;
    top: 50%;
    width: 100%;
    
    &:after {
      background-color: #6ec0cd;
      content: '';
      height: 100%;
      position: absolute;
      top: 0;
      transition: all $transition-time;
    }
  }
  
  &-top {
    transform: rotate(45deg);
    transform-origin: bottom right;
    
    &:after {
      left: 100%;
      right: 0;
      transition-delay: 0s;
    }
  }
  
  &-bottom {
    transform: rotate(-45deg);
    transform-origin: top right;
    
    &:after {
      left: 0;
      right: 100%;
      transition-delay: $transition-time;
    }
  }
  
  &:hover & {
    
    &-top:after {
      left: 0;
      transition-delay: $transition-time;
    }

    &-bottom:after {
      right: 0;
      transition-delay: 0s;
    }
  }
}
</style>