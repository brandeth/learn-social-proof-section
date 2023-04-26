<script lang="ts" setup>
defineProps<{
  card: Card
}>()
</script>

<template>
  <div class="SocialProofSection-cardItem">
    <div class="CardItem-header">
      <div class="CardItem-headerImage">
        <img :src="card.avatar" alt="Colton Smith">
      </div>
      <div class="CardItem-headerText">
        <h3>{{ card.name }}</h3>
        <p v-if="card.isVerified">Verified Buyer</p>
      </div>
    </div>
    <div class="CardItem-body">
      <p>{{ card.review }}</p>
    </div>
  </div>
</template>