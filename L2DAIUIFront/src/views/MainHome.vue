<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Home</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <AlarmClockSetup></AlarmClockSetup>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import AlarmClockSetup from '@/modules/AlarmClockModule/components/AlarmClockSetup.vue';
</script>
