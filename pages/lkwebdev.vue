<template>
  <div class="blocks">
    <div id="firstBlock" class="block">
      <div class="overlay"></div>
      <FirstBlock />
    </div>
    <div id="secondBlock" class="block">
      <SecondBlock />
    </div>
    <!-- <div id="thirdBlock" class="block full-height">
      <ThirdBlock />
    </div>
    <div id="fourthBlock" class="block full-height">
      <FourthBlock />
    </div> -->
  </div>
</template>

<script>
import FirstBlock from '@/components/LKWebDev/FirstBlock/FirstBlock.vue'
import SecondBlock from '@/components/LKWebDev/SecondBlock/SecondBlock.vue'

export default {
  components: {
    FirstBlock,
    SecondBlock
  }
}
</script>

<style>
  @font-face {
    font-family: 'Lato Regular';
    src: url('@/assets/fonts/Lato-Regular.ttf');
  }

  @font-face {
    font-family: 'Lato Bold';
    src: url('@/assets/fonts/Lato-Bold.ttf');
  }

  body {
    font-family: 'Lato Regular';
  }
  h1 ,h2, h3, h4 {
    font-family: 'Lato Bold';
  }
  p {
    font-size: 18px;
  }
  .container {
    max-width: 1280px;
  }
  #header {
    position: relative!important;
  }
  .block.full-height {
    min-height: 100vh;
  }
  .overlay {
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    background: rgba(0,0,0,0.66);
    z-index: -1;
  }
</style>
