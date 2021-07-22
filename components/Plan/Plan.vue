<template>
  <div class="plan">
    <div class="plan__price-box">
      <span class="plan__price">
        £{{ price }}
      </span>
    </div>
    <div class="plan__header">
      <h4><span v-html="name" /></h4>
    </div>
    <div class="plan__features">
      <div class="plan__feature hide-text">
        {{ features }}
      </div>
      <a class="see-more" @click="expandText">See more</a>
    </div>
    <div class="coming_soon_overlay">
      <span>Coming soon!</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Plan',
  props: {
    plan: {
      type: Object,
      required: true
    }
  },
  computed: {
    name () {
      return this.plan.name
    },
    price () {
      return this.plan.price
    },
    features () {
      return this.plan.features
    },
    seemore () {
      return this.plan.name.toLowerCase().trim()
    }
  },
  methods: {
    expandText (event) {
      const textContainer = event.target.previousSibling.previousSibling

      if (textContainer.className.includes('hide-text')) {
        textContainer.classList.add('show-text')
        textContainer.classList.remove('hide-text')
      } else {
        textContainer.classList.add('hide-text')
        textContainer.classList.remove('show-text')
      }
    }
  }
}
</script>

<style>
.plan__table {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: flex-start;
}
.plan {
  flex: 1;
  padding: 1.5rem 1rem 2rem 1rem;
  margin: 1rem;
  background: #fff;
  border-radius: 8px;
  box-shadow: 0 8px 12px 0 rgba(122,122,122,0.2);
  transition: opacity 500ms linear,
  transform 250ms ease-in-out;
  overflow: hidden;
  text-overflow: ellipsis;
  align-self: flex-start;
  position: relative;
}

.plan:hover {
  transform: scale(1.05) translateZ(0);
  backface-visibility: hidden;
}

.plan__price {
    font-size: 3rem;
}

.plan__feature {
    font-size: 0.9rem;
    text-overflow: ellipsis;
    padding-bottom: 2rem;
    transition: max-height 5s linear;
    overflow: hidden;
    max-height: 10.5rem;
}

.plan__feature.show-text {
  max-height: unset;
}

.coming_soon_overlay {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  background: rgba(0,0,0,0.95);
  font-size: 2.5rem;
  padding: 1rem 0;
  white-space: nowrap;
}

.coming_soon_overlay span {
  color: #fff;
  position: absolute;
  top:40%;
  left: 0;
  right: 0;
}

@media (max-width: 1400px) {
    .plan__table {
        flex-direction: column;
    }
}
</style>
