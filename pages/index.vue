<template>
  <div class="landingPageContainer d-flex align-items-center justify-content-center text-align-center">
    <div class="container">
      <div class="row">
        <div class="col">
          <div class="textEffect">
            <p>I am</p>
            <b>
              <div class="textToScroll">
                <div v-for="(text, index) in scrollText" :key="index">
                  {{ text }}<br />
                </div>
              </div>
            </b>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col">
          <div class="description">
            <p>I am a software engineer with years of experience in FinTech, Supply Chain, and other various management systems.</p>
            <p>You'd also often find me organizing and being heavily involved in events for geeks, learners, empowerment, and equality.</p>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col">
          <a class="btn btn-light custom-buttons" v-b-tooltip.hover title="Coming Soon!">See My Works</a>
          <a class="btn btn-outline-light custom-buttons secondary" href="http://www.linkedin.com/in/iyahnuestro" target="_blank">Contact Me</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  data() {
    return {
      scrollText: ['Iyah Nuestro.', 'a Software Engineer.', 'a puzzle-lover.', 'customer-centric.', 'radical.']
    }
  },
  head () {
    return {
      title: 'Iyah Nuestro',
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        { hid: 'description', name: 'description', content: 'Software Engineer' }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.landingPageContainer {
  height: 100vh;
  .title {
    color: white;
    font-family: 'Fira Sans', sans-serif;
  }
  .textEffect {
    font: normal 40px/50px 'Fira Sans', sans-serif;
    color: white;
    p {
      height: 50px;
      float: left;
      margin-right: 0.3em;
    }
    b {
      float: left;
      overflow: hidden;
      position: relative;
      height: 50px;
      top: 0px;
    }
    .textToScroll {
      display: inline-block;
      color: white;
      opacity: 0.75;
      position: relative;
      white-space: nowrap;
      top: 0;
      left: 0;

      /*animation*/
      -webkit-animation: move 10s;
      -moz-animation: move 10s;
      -ms-animation: move 10s;
      -o-animation: move 10s;
      animation: move 10s;
      /*animation-iteration-count*/
      -webkit-animation-iteration-count: infinite;
      -moz-animation-iteration-count: infinite;
      -ms-animation-iteration-count: infinite;
      -o-animation-iteration-count: infinite;
      animation-iteration-count: infinite;
      /*animation-delay*/
      -webkit-animation-delay: 10s;
      -moz-animation-delay: 10s;
      -ms-animation-delay: 10s;
      -o-animation-delay: 10s;
      animation-delay: 10s;
    }
    @keyframes move {
      0% {
        top: 0px;
      }
      20% {
        top: -50px;
      }
      40% {
        top: -100px;
      }
      60% {
        top: -150px;
      }
      80% {
        top: -200px;
      }
    }
    @-webkit-keyframes move {
      0% {
        top: 0px;
      }
      20% {
        top: -50px;
      }
      40% {
        top: -100px;
      }
      60% {
        top: -150px;
      }
      80% {
        top: -200px;
      }
    }
    @-moz-keyframes move {
      0% {
        top: 0px;
      }
      20% {
        top: -50px;
      }
      40% {
        top: -100px;
      }
      60% {
        top: -150px;
      }
      80% {
        top: -200px;
      }
    }
    @-o-keyframes move {
      0% {
        top: 0px;
      }
      20% {
        top: -50px;
      }
      40% {
        top: -100px;
      }
      60% {
        top: -150px;
      }
      80% {
        top: -200px;
      }
    }
    @keyframes move {
      0% {
        top: 0px;
      }
      20% {
        top: -50px;
      }
      40% {
        top: -100px;
      }
      60% {
        top: -150px;
      }
      80% {
        top: -200px;
      }
    }
  }
  .description {
    color: white;
    font-family: 'Fira Sans', sans-serif;
    padding-top: 24px;
  }
  .custom-buttons {
    font-family: 'Fira Sans', sans-serif;
    margin-top: 48px;
    &.secondary {
      color: white;
      &:hover {
        color: black;
      }
    }
  }
}
</style>
