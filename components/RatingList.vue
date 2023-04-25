<script lang="ts" setup>
const ratings = ref<Rating[]>([
  {
    value: 5,
    channel: 'Reviews'
  },
  {
    value: 5,
    channel: 'Report Guru'
  },
  {
    value: 5,
    channel: 'BestTech'
  },
])
</script>

<template>
  <div class="SocialProofSection-ratingList">
    <RatingItem v-for="(rating, index) in ratings" :key="index" :rating="rating" />
  </div>
</template>