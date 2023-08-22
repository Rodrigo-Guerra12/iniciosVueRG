<template>
  <div class="rating">
    <span
      v-for="(star, index) in stars"
      :key="index"
      class="star"
      :class="{ 'filled': index < currentRating }"
      @click="setRating(index + 1)"
    >
      &#9733;
    </span>
  </div>
</template>

<script>
export default {
  props: {
    maxRating: {
      type: Number,
      default: 5,
    },
    initialRating: {
      type: Number,
      default: 0,
    },
  },
  data() {
    return {
      currentRating: this.initialRating,
      stars: new Array(this.maxRating),
    };
  },
  methods: {
    setRating(rating) {
      this.currentRating = rating;
      this.$emit('rating-selected', rating);
    },
  },
};
</script>

<style scoped>
.rating {
  display: inline-block;
  font-size: 1.5rem;
}

.star {
  cursor: pointer;
}

.filled {
  color: gold;
}
</style>
