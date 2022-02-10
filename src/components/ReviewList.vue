<template>
  <div>
    <review-item v-for="review in reviews"
                 :review="review"
                 :key="review.id"
    />
  </div>
</template>

<script>
import ReviewItem from "./ReviewItem";

export default {
  components: {ReviewItem},
  props: {
    reviews: {
      type: Array,
      required: true
    }
  }
}
</script>

<style scoped>

</style>