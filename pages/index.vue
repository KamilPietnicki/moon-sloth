<template>
  <div class="container">
    <LandingContent />
    <div class="content-wrap">
      <Header />    
      <MainContent />
    </div>
  </div>
</template>

<script>
import LandingContent from '~/components/LandingContent.vue'
import Header from '~/components/Header.vue'
import MainContent from '~/components/MainContent.vue'

export default {
  components: {
    LandingContent,
    Header,
    MainContent
  },

  methods: {
    beforeAppear: function(el) {
      console.log('beforeAppear')
    },
    appear: function(el) {
      console.log('appear!')
    },
    afterAppear: function(el) {
      console.log('afterAppear!')
    } 
  }
}
</script>

<style lang="scss">
.container {
  display: block;
  position: relative;
  margin: 0 auto;
  min-height: 100vh;
  width: 100%;
}

.content-wrap {
  display: block;
  position: relative;

  width: calc(100% - 160px);
  max-width: 1440px;
  min-height: 100vh;
  margin: 0 auto;
}

h1, h2, h3, p, a, span {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
}

.title {
  display: block;
  font-weight: 300;
  font-size: 55px;
  color: #35495e;
  letter-spacing: 1px;
  text-transform: capitalize;
  margin: 25px 0;

  @media (max-width: 767.98px){
  	font-size: 2.2rem;
  }
}

.subtitle {
  font-weight: 300;
  font-size: 1.1rem;
  color: #526488;
  word-spacing: 2px;
  padding-bottom: 15px;
  max-width: 600px;
}

.subtitle a {
  font-weight: 500;
  color: inherit;
}

.links {
  padding-top: 15px;
  margin-bottom: 20px;
}

.content-logos {
  display: flex;
  align-items: center;
  justify-content: center;
  min-width: 500px;
}

.plus {
  font-size: 2.5rem;
  margin: 15px;
  color: #35495e;
}

.h3 {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-weight: 400;
  margin: 0px;
}

.fade-enter-active {
  animation: go 2s;
}

@keyframes go {
  from {
    background: #fff;
  }
  to {
    background: #999;
  }
}
</style>
