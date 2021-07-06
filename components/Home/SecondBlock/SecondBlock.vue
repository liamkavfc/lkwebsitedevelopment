/* eslint-disable vue/no-unused-components */
<template>
  <div>
    <div class="container d-flex flex-row text-center">
      <div class="p-2 flex-fill">
        <b-icon-calendar-3 scale="6" />
        <br><br>
        <h3 class="mt-md-3">Speedy Turnaround</h3>
        <p>Our templated approach offers a quick turnaround</p>
      </div>
      <div class="p-2 flex-fill">
        <b-icon-people scale="6" />
        <br><br>
        <h3 class="mt-md-3">Small Businesses</h3>
        <p>Primarily targeting small business to help their online presence</p>
      </div>
      <div class="p-2 flex-fill">
        <b-icon-chat scale="6" />
        <br><br>
        <h3 class="mt-md-3">Friendly &amp; Transparent</h3>
        <p>Happy to help and always 100% transparent communication</p>
      </div>
    </div>
  </div>
</template>

<script>
import { BIconCalendar3, BIconPeople, BIconChat } from 'bootstrap-vue'

export default {
  name: 'SecondBlock',
  components: {
    BIconCalendar3,
    BIconPeople,
    BIconChat
  }
}
</script>

<style>
  #secondBlock {
    background: #eee;
    padding: 7.5rem 0;
  }

  @media (max-width: 600px) {
    #secondBlock {
      padding: 2rem 0;
    }

    #secondBlock svg {
      height: 0.5rem;
      width: 0.5rem;
    }

    #secondBlock h3 {
      font-size: 0.9rem;
    }

    #secondBlock p {
      font-size: 0.7rem;
    }
  }

</style>
