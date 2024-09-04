<template>
    <div>
      <!-- add alarm card -->
      <ion-card>
      <ion-card-header>
        <ion-row>
          <ion-col class="ion-margin-start">
            <ion-card-title>Add alarm</ion-card-title>
          </ion-col>
          <ion-col class="ion-margin-end">
            <ion-button id="open-modal" size="large">
              <ion-icon slot="icon-only" :icon="add"></ion-icon>
            </ion-button>
          </ion-col>
        </ion-row>
      </ion-card-header>
    </ion-card>
    <!-- add alarm modal -->
    <!-- alarms data -->
    <ion-card>
      <ion-card-header>
        <ion-card-title>Alarms list</ion-card-title>
      </ion-card-header>
      <ion-list>
        <ion-item>
          <ion-thumbnail slot="start">
            <img alt="Silhouette of mountains" src="https://ionicframework.com/docs/img/demos/thumbnail.svg" />
          </ion-thumbnail>
          <ion-label>Item</ion-label>
        </ion-item>
      </ion-list>
    </ion-card>
    </div>
  </template>
  
  <script lang="ts">
   import { add } from 'ionicons/icons';
   import { ref } from 'vue'
   export default {
     setup() {
        // var declarations
        const alarmsQuantity = ref([])
        const modal = ref();
        return {
          // components
          add,
          /* var data exposed to template */
          modal,
          alarmsQuantity
        };
   },
  };
  </script>