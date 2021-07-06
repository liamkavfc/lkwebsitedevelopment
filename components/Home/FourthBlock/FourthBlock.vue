<template>
  <div class="col-md-8 offset-md-2 services">
    <h1 class="text-center mb-5">
      Services
    </h1>
    <b-row>
      <b-col md="4" sm="12" class="mb-3">
        <div class="text-center">
          <h3>LK Web Development</h3>
          <br>
          <img src="~/assets/images/logo_black.png" style="width: 96px;" />
          <br><br>
          <p>I can help you build, ammend or even something simple like answer any questions you may have. Please get in touch to see how I can help you reach your online potential!</p>
        </div>
      </b-col>
      <b-col md="4" sm="12" class="mb-3">
        <div class="text-center">
          <h3>Collabs</h3>
          <br><br>
          <b-icon-people-fill scale="6" />
          <br><br><br><br>
          <p>Im always open for the possiblility of working with other developers on fun project or even designers on website projects. Please do get in touch to see how we can team up!</p>
        </div>
      </b-col>
      <b-col md="4" sm="12" class="mb-3">
        <div class="text-center">
          <h3>Get in touch</h3>
          <br><br>
          <b-icon-linkedin scale="6" />
          <br><br><br><br>
          <p>The best way to contact me about the points I have mentioned is LinkedIn. Come connect with me and lets chat!</p>
        </div>
      </b-col>
    </b-row>
  </div>
</template>

<script>
import { BIconPeopleFill, BIconLinkedin } from 'bootstrap-vue'

export default {
  name: 'FourthBlock',
  components: {
    BIconPeopleFill,
    BIconLinkedin
  }
}
</script>

<style>
  #fourthBlock {
    background: #eee;
    padding: 7.5rem 0;
  }
</style>
