<template>
  <div class="text-center">
    <img class="img-fluid d-block d-sm-none" src="~/assets/images/lkbanner.jpg" />
    <img class="img-fluid d-none d-sm-inline-block" src="~/assets/images/lkbanner_desktop.jpg" />
  </div>
</template>

<script>
export default {
  name: 'BannerBlock'
}
</script>

<style>

  #BannerBlock {
    background-color: rgba(0, 0, 0, 0.75);
  }

  #BannerBlock .details {
    padding-top: 20vh;
    z-index: 99;
  }

  #BannerBlock .details .profile_image {
    height: 300px;
    width: 300px;
    border-radius: 45rem;
    background-image: url('@/assets/images/selfimage-2.JPG');
    background-size: 225%;
    background-repeat: no-repeat;
    background-position: 43% 50%;
    margin: auto;
    box-sizing: border-box;
    -moz-box-sizing: border-box;
    -webkit-box-sizing: border-box;
    border: 8px solid rgba(0, 0, 0, 0.75);
  }

  #BannerBlock .details .profile_name {
      padding: 2rem 0;
  }

  #BannerBlock .details .profile_name * {
    color: #fff;
  }
</style>
