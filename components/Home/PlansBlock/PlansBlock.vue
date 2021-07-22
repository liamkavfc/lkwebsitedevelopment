<template>
  <div id="prices" class="col-md-8 offset-md-2 text-center">
    <h1 class="mb-5">
      Prices
    </h1>
    <b-container>
      <div class="plan__table">
        <Plan
          v-for="(plan, index) in plans"
          :key="index"
          :plan="plan"
          :data-index="index"
        />
      </div>
    </b-container>
  </div>
</template>

<script>
import Plan from '@/components/Plan/Plan.vue'

export default {
  name: 'PlansBlock',
  components: {
    Plan
  },
  data () {
    return {
      plans: [
        {
          name: 'Static Single Page<br />Template',
          price: 100,
          features: 'Just a single page static website. We will help you get started with web hosting, domain names etc. We can then provide the website files we have made for you and upload them to the web hosting company you have chosen to go with (GoDaddy etc). Once files have been handed over and uploaded, this service will be complete. If you require any further changes, that would come under the \'Website Tweaks\' service.'
        },
        {
          name: 'Static Multi Page<br />Template',
          price: 150,
          features: 'Similar to the first option but instead of having all your content on one page, it will be split accross multiple pages with the links in the header taking you those. We will help you get started with web hosting, domain names etc. We can then provide the website files we have made for you and upload them to the web hosting company you have chosen to go with (GoDaddy etc). Once files have been handed over and uploaded, this service will be complete. If you require any further changes, that would come under the \'Website Tweaks\' service.'
        },
        {
          name: 'Wix<br />CMS Website',
          price: 200,
          features: 'Website hosted on Wix which includes setting up your domain name all done through Wix. We will get you started by getting all your content into Wix, help setting up your Wix account, getting your domain name sorted, choosing a template etc. Using Wix means you can update your content on your website yourself through the Wix site editor which we can fully support you with to get you more familiar. This will allow you to upload images, add pages, add your own text and more! Once you are happy with your site, the service will be complete. If you require any further changes, that would come under the \'Website Tweaks\' service.'
        }
      ]
    }
  }
}
</script>

<style>
  #PlansBlock {
    background: #eee;
    padding: 2rem 0;
  }

  #PlansBlock a {
    color: #000;
  }
</style>
