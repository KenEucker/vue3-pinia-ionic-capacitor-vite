<script setup lang="ts">
import { defineEmits } from 'vue'
import {
  IonContent,
  IonButton,
  IonButtons,
  // IonBackButton,
  IonHeader,
  IonTitle,
  IonToolbar,
} from '@ionic/vue'
const emit = defineEmits(['onClose'])
</script>

<template>
  <ion-header>
    <ion-toolbar>
      <ion-buttons>
        <ion-button @click="emit('onClose')">CLOSE</ion-button>
      </ion-buttons>
      <ion-title>About Modal</ion-title>
    </ion-toolbar>
  </ion-header>
  <ion-content class="ion-padding">
    <h1>THIS IS MY MODAL</h1>
  </ion-content>
</template>
