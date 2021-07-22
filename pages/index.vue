<template>
  <div class="blocks">
    <div id="BannerBlock" class="block">
      <BannerBlock />
    </div>
    <div id="AboutBlock" class="block">
      <AboutBlock />
    </div>
    <div id="WorkBlock" class="block">
      <WorkBlock />
    </div>
    <div id="PlansBlock" class="block">
      <PlansBlock />
    </div>
    <div id="ContactBlock" class="block">
      <ContactBlock />
    </div>
  </div>
</template>

<script>
import BannerBlock from '@/components/Home/BannerBlock/BannerBlock.vue'
import AboutBlock from '@/components/Home/AboutBlock/AboutBlock.vue'
import WorkBlock from '@/components/Home/WorkBlock/WorkBlock.vue'
import ContactBlock from '@/components/Home/ContactBlock/ContactBlock.vue'
import PlansBlock from '@/components/Home/PlansBlock/PlansBlock.vue'

export default {
  components: {
    BannerBlock,
    AboutBlock,
    WorkBlock,
    ContactBlock,
    PlansBlock
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

  .blocks > .block:nth-child(odd) {
    background: #fff;
  }

  .blocks > .block:nth-child(even) {
    background: #eee;
  }
</style>
