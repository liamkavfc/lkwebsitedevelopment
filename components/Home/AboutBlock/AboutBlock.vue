<template>
  <div>
    <div class="container col-12 text-center">
      <div class="row">
        <div class="p-2 col-6 col-sm-4">
          <b-icon-calendar-3 scale="6" />
          <br><br>
          <h3 class="mt-md-3">Speedy Turnaround</h3>
          <p>Our templated approach offers a quick turnaround</p>
        </div>
        <div class="p-2 col-6 col-sm-4">
          <b-icon-people scale="6" />
          <br><br>
          <h3 class="mt-md-3">Small Businesses</h3>
          <p>Primarily targeting small business to help their online presence</p>
        </div>
        <div class="p-2 col-6 col-sm-4 offset-3 offset-sm-0">
          <b-icon-chat scale="6" />
          <br><br>
          <h3 class="mt-md-3">Friendly &amp; Transparent</h3>
          <p>Happy to help and always 100% transparent communication</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { BIconCalendar3, BIconPeople, BIconChat } from 'bootstrap-vue'

export default {
  name: 'AboutBlock',
  components: {
    BIconCalendar3,
    BIconPeople,
    BIconChat
  }
}
</script>

<style>
  #AboutBlock {
    padding: 7.5rem 0;
  }

  @media (max-width: 600px) {
    #AboutBlock {
      padding: 2rem 0;
    }

    #AboutBlock svg {
      height: 0.5rem;
      width: 0.5rem;
    }

    #AboutBlock h3 {
      font-size: 0.9rem;
    }

    #AboutBlock p {
      font-size: 0.7rem;
    }
  }

</style>
