<template>
    <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Meus contatos</ion-title>
      </ion-toolbar>
    </ion-header>
    
    <ion-content >
      <ion-list>
        <ion-toolbar>
          <ion-item v-for="list in arrayLista" :key="list">
           <ion-label>{{list}}</ion-label>
          </ion-item>
        </ion-toolbar>
      </ion-list>
    
    </ion-content>
  </ion-page>
</template>

<script>
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar,IonItem,IonLabel,IonList } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Home',
  components: {
    IonContent,
    IonHeader,
    IonPage,
    IonTitle,
    IonToolbar,IonItem,IonLabel,IonList
  },
  setup() {
      return{
          arrayLista:["Helton","Elisa","Pardal"]
      }
  }
});
</script>

<style scoped>

</style>