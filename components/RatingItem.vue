<script lang="ts" setup>
defineProps<{
  rating: Rating
}>()
</script>

<template>
  <div class="SocialProofSection-ratingItem">
    <div class="Rating-starContainer">
      <img src="/icon-star.svg" v-for="n in rating.value" :key="n" />
    </div>
    <p class="Rating-channel">Rated {{ rating.value }} Stars in {{ rating.channel }}</p>
  </div>
</template>
