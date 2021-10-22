<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title> {{ title }} </ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content>
      <slot />
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import {
  IonHeader,
  IonTitle,
  IonContent,
  IonToolbar,
  IonPage,
} from "@ionic/vue";
import { defineComponent } from "vue";

export default defineComponent({
  components: {
    IonContent,
    IonTitle,
    IonHeader,
    IonToolbar,
    IonPage,
  },

  props: {
    title: String,
  },
});
</script>
