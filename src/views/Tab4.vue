<template>
  <ion-page>
      <ion-content>
          <ion-input :value="name" type="text" placeholder="Awesome Input"></ion-input>
          <ion-card>
            <ion-card-header>
            <ion-img :src="imgLoc"></ion-img> 

              <ion-card-subtitle>Jorge</ion-card-subtitle>
              <ion-card-title>CEO</ion-card-title>
            </ion-card-header>
            <ion-card-content>
              HOLI
            </ion-card-content>
          </ion-card>
          <ion-checkbox></ion-checkbox>
      <h1>HOLA {{name}}</h1>
      </ion-content>
    </ion-page>
</template>

<script>
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';
import ExploreContainer from '@/components/ExploreContainer.vue';

export default  {
        data() {
        return {

            name: "Oleg",
            imgLoc: "https://upload.wikimedia.org/wikipedia/commons/e/ef/Paquirr%C3%ADn.jpg"
        }
    },
  name: 'Tab3',
  components: {  IonContent, IonPage },
  created(){
    console.log("HOLA MUNDO");
    
  }
  
}

</script>

<style>

</style>