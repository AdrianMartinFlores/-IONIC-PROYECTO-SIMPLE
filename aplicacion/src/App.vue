<template>
  <ion-menu content-id="main-content">
    <ion-header>
      <ion-toolbar>
        <ion-title> CONTENIDO</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content class="ion-padding">
      <ion-link router-link="/vuelos">
        <ion-button color="primary">
          <ion-icon slot="start" name="home"></ion-icon>
          Vuelos
        </ion-button>
        </ion-link>
        <br>
        <ion-link router-link="/reservas">
        <ion-button color="primary">
          <ion-icon slot="start" name="home"></ion-icon>
          Reservas
        </ion-button>
      </ion-link>
      <br>
      <ion-link router-link="/usuario">
        <ion-button color="primary">
          <ion-icon slot="start" name="home"></ion-icon>
          Usuario
        </ion-button>
      </ion-link>
    </ion-content>
  </ion-menu>
  <ion-page id="main-content">
    <ion-header>
      <ion-toolbar>
        <ion-buttons slot="start">
          <ion-menu-button></ion-menu-button>
        </ion-buttons>
        <ion-title>Menu</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content class="ion-padding">
      <ion-title class="titulo">RESERVA AHORA TUS VUELOS</ion-title>
      <p class="descripcion">Reserva ahora tus vuelos y obtén un descuento de hasta 20% en tus próximos viajes.</p>
      <div class="caja-imagen">
        <ion-card class="">
          <img alt="Silhouette of mountains" src="https://fotografias.larazon.es/clipping/cmsimages02/2024/01/24/7523015D-F5DF-4A1D-9FBF-A125655508A9/calcula-que-dia-producen-120000-vuelos-aunque-numero-puede-ser-mayor_98.jpg?crop=4242,2387,x0,y221&width=1900&height=1069&optimize=low&format=webply" />
          <ion-card-header>
            <ion-card-title>Vuelos</ion-card-title>
            <ion-card-subtitle>Reserva tus vuelos</ion-card-subtitle>
          </ion-card-header>
          <ion-card-content>
            <ion-button expand="block" color="primary" router-link="/vuelos">Reservar vuelo</ion-button>
          </ion-card-content>
        </ion-card>
      </div>
      <ion-card color="primary">
  <ion-card-header>
    <ion-card-title>Vuelos baratos </ion-card-title>
    <ion-card-subtitle>Los precios más asequibles  </ion-card-subtitle>
  </ion-card-header>

</ion-card>
<ion-card style="background-color: green;">
  <ion-card-header>
    <ion-card-title style="color: white;">Vuelos corta distancia</ion-card-title>
    <ion-card-subtitle style="color: white;">Vuelos a menos de 100 km</ion-card-subtitle>
  </ion-card-header>

</ion-card>
<ion-card style=" background-color: red;">
  <ion-card-header>
    <ion-card-title style="color: white;">Vuelos a larga distancia</ion-card-title>
    <ion-card-subtitle style="color: white;">Vuelos a más de 100 km</ion-card-subtitle>
  </ion-card-header>
  <ion-card-content> Card Content </ion-card-content>
</ion-card>

    </ion-content>
  </ion-page>
  <ion-router-outlet></ion-router-outlet>
</template>

<script lang="ts">
import { IonButtons, IonContent, IonHeader, IonMenu, IonMenuButton, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
</script>
<style scoped>
.titulo {
  font-size: 50px;
  color: black;
  text-align: center;
}

.descripcion {
  font-size: 20px;
  color: black;
  text-align: center;
}

.imagen {
  width: 10%;


}

.caja-imagen {
  display: flex;
  justify-content: center;
  align-items: center;  
  margin-top: 10%;
  margin-bottom: 10%;
  margin-left: 25%;
  margin-right: 25%;
  box-shadow: 0 0 10px #888888;
}
</style>