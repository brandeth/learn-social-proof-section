<script lang="ts" setup>
interface Rating {
  rating: number
  channel: string
}

const ratings = ref<Rating[]>([
  {
    rating: 5,
    channel: 'Reviews'
  },
  {
    rating: 5,
    channel: 'Report Guru'
  },
  {
    rating: 5,
    channel: 'BestTech'
  },
])
</script>

<template>
  <div class="SocialProofSection-ratingList">
    <RatingItem v-for="(rating, index) in ratings" :key="index" :rating="rating" />
  </div>
</template>