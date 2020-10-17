<template>
  <ion-page>
    <ion-content>
      <ExploreContainer :name="welcome" />
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import ExploreContainer from '@/components/ExploreContainer.vue';
import { IonPage } from '@ionic/vue';
import { ellipse, square, triangle, accessibilityOutline } from 'ionicons/icons';

export default {
  name: 'Home',
  components: {IonPage, ExploreContainer },

  setup() {
    return {
      ellipse, 
      square, 
      triangle,
      accessibilityOutline,
      welcome: "¡Bienvenido Oleg!",
    }
  }
}
</script>