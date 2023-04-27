<script lang="ts" setup>
useHead({
  title: "Social Proof Section - Frontend Mentor | Rey Garcia",
  meta: [
    {
      name: "description",
      content: "Social Proof Section",
    },
  ],
});
</script>

<template>
  <div class="SocialProofSection">
    <div class="SocialProofSection-header">
      <Overview />
      <RatingList />
    </div>
    <CardList />
  </div>
</template>
