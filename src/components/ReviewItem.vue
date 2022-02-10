<template>
  <v-card class='review'>
    <v-avatar color="primary" size="80">
      <img :src="review.img" :alt="review.name">
    </v-avatar>
  </v-card>
</template>

<script>
export default {
  props: {
    review: {
      type: Object,
      required: true
    }
  }
}
</script>

<style lang='scss' scoped>
.review {
  display: flex;
  gap: 30px;
  align-items: flex-start;
  padding: 35px 40px;
  background: #FFFFFF;
  border-radius: 4px;

  &:not(:last-child) {
    margin: 0 0 15px;
  }
}
</style>