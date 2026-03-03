<script setup>
import AnnouncementBanner from '@/components/AnnouncementBanner.vue'
import LandingPage from '@/components/LandingPage.vue'
import LineupPage from '@/components/LineupPage.vue'
import WayfindPage from '@/components/WayfindPage.vue';
</script>

<template>
  <LandingPage id="home" />
  <LineupPage id="lineup" />
  <AnnouncementBanner id="announcement" />
  <WayfindPage id="wayfind" />
</template>
