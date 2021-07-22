<template>
  <div id="contact" class="col-md-8 offset-md-2 text-center">
    <h1 class="mb-5">
      Contact Us
    </h1>
    <b-container>
      <b-row>
        <b-col sm="6" class="mb-4">
          <a href="https://www.facebook.com/LKWebDevelopment">
            <b-icon-facebook scale="6"></b-icon-facebook>
            <h3 class="mt-5">Facebook</h3>
            <p>LKWebDevelopment</p>
          </a>
        </b-col>
        <b-col sm="6" class="mb-4">
          <a href="https://www.instagram.com/lkwebsitedevelopment/">
            <b-icon-instagram scale="6"></b-icon-instagram>
            <h3 class="mt-5">Instagram</h3>
            <p>@lkwebsitedevelopment</p>
          </a>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import { BIconFacebook, BIconInstagram } from 'bootstrap-vue'

export default {
  name: 'ContactBlock',
  components: {
    BIconFacebook,
    BIconInstagram
  }
}
</script>

<style>
  #ContactBlock {
    padding: 2rem 0;
  }

  #ContactBlock a {
    color: #000;
  }
</style>
