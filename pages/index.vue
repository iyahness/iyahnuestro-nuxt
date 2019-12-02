<template>
  <div class="landingPageContainer d-flex align-items-center justify-content-center text-align-center">
    <div class="container">
      <div class="row">
        <div class="col">
          <div class="textEffect">
            <p>I am</p>
            <b>
              <div class="textToScroll">
                Iyah Nuestro.<br /> 
                a Software Engineer.<br />
                a puzzle-lover.<br />
                customer-centric.
                </div>
            </b>
          </div>
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
    padding: 2em 5em;
    font: normal 40px/50px Montserrat, sans-serif;
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
      color: #e74c3c;
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
      -webkit-animation-delay: 3s;
      -moz-animation-delay: 3s;
      -ms-animation-delay: 3s;
      -o-animation-delay: 3s;
      animation-delay: 3s;
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
</style>
