<template>
    <ion-menu side="end" content-id="main-content">
        <ion-header>
            <ion-toolbar>
                <ion-title>Menu</ion-title>
            </ion-toolbar>
        </ion-header>
        <ion-content class="ion-padding">
            <ion-list>
                <ion-item>
                    <ion-label>Test</ion-label>
                </ion-item>
            </ion-list>
        </ion-content>
    </ion-menu>
    <ion-page id="main-content">
        <ion-header>
            <ion-toolbar>
                <ion-title>Tab 1</ion-title>
                <ion-buttons slot="end">
                    <ion-menu-button></ion-menu-button>
                </ion-buttons>
            </ion-toolbar>
        </ion-header>
        <ion-content :fullscreen="true">
            <ion-header collapse="condense">
                <ion-toolbar>
                    <ion-title size="large">Tab 1</ion-title>
                </ion-toolbar>
            </ion-header>

            <ExploreContainer name="Tab 1 page" />
        </ion-content>
    </ion-page>
</template>

<script setup lang="ts">
import {
    IonPage,
    IonHeader,
    IonToolbar,
    IonTitle,
    IonContent,
    IonMenu,
    IonMenuButton,
    IonList,
    IonItem,
    IonLabel,
    IonButtons,
    IonButton,
} from "@ionic/vue";
import ExploreContainer from "@/components/ExploreContainer.vue";
</script>
