<script lang="ts" setup>
const cardList = ref<Card[]>([
  {
    avatar: 'image-colton.jpg',
    name: 'Colton Smith',
    isVerified: true,
    review: '“ We needed the same printed design as the one we had ordered a week prior. Not only did they find the original order, but we also received it in time. Excellent! ”',
  },
  {
    avatar: 'image-irene.jpg',
    name: 'Irene Roberts',
    isVerified: true,
    review: '“ Customer service is always excellent and very quick turn around. Completely delighted with the simplicity of the purchase and the speed of delivery. ”',
  },
  {
    avatar: 'image-anne.jpg',
    name: 'Anne Wallace',
    isVerified: true,
    review: '“ Put an order with this company and can only praise them for the very high standard. Will definitely use them again and recommend them to everyone! ”',
  },
])
</script>

<template>
  <div class="SocialProofSection-cardList">
    <CardItem v-for="(card, index) in cardList" :key="index" :card="card" />
  </div>
</template>