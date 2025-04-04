<template>
  <ion-page class="mt-20">
    <ion-content :fullscreen="true">
      <div id="container">
        <ion-list id="list">
          <ion-item>
            <ion-img src="vaca.webp"></ion-img>
            <ion-label class="m-2 text-sm">
              <h2>Vaca</h2>
              <p>MUUUUUUUUUH</p>
            </ion-label>
            <ion-button slot="end" fill="outline" @click="playSound('vaca-sonido.mp3')">
              <play-button/>
            </ion-button>
          </ion-item>
          <ion-item>
            <ion-img src="oveja.webp"></ion-img>
            <ion-label class="m-2 text-sm">
              <h2>Oveja</h2>
              <p>BEEEHHHHHH</p>
            </ion-label>
            <ion-button slot="end" fill="outline" @click="playSound('oveja-sonido.mp3')">
              <play-button/>
            </ion-button>
          </ion-item>
          <ion-item>
            <ion-img src="cerdo.webp"></ion-img>
            <ion-label class="m-2 text-sm">
              <h2>Cerdo</h2>
              <p>Oing oing</p>
            </ion-label>
            <ion-button slot="end" fill="outline" @click="playSound('cerdo-sonido.mp3')">
              <play-button/>
            </ion-button>
          </ion-item>
          <ion-item>
            <ion-img src="gallina.jpeg"></ion-img>
            <ion-label class="m-2 text-sm">
              <h2>Gallina</h2>
              <p>quiquiriqui</p>
            </ion-label>
            <ion-button slot="end" fill="outline" @click="playSound('gallina-sonido.mp3')">
              <play-button/>
            </ion-button>
          </ion-item>
          <ion-item>
            <ion-img src="pato.jpeg"></ion-img>
            <ion-label class="m-2 text-sm">
              <h2>Pato</h2>
              <p>CUACK!</p>
            </ion-label>
            <ion-button slot="end" fill="outline" @click="playSound('pato-sonido.mp3')">
              <play-button/>
            </ion-button>
          </ion-item>
          <ion-item>
            <ion-img src="perro.jpeg"></ion-img>
            <ion-label class="m-2 text-sm">
              <h2>Perro</h2>
              <p>Guau!</p>
            </ion-label>
            <ion-button slot="end" fill="outline" @click="playSound('perro-sonido.mp3')">
              <play-button/>
            </ion-button>
          </ion-item>
          <ion-item>
            <ion-img src="gato.jpg"></ion-img>
            <ion-label class="m-2 text-sm">
              <h2>Gato</h2>
              <p>MIAU</p>
            </ion-label>
            <ion-button slot="end" fill="outline" @click="playSound('gato-sonido.mp3')">
              <play-button/>
            </ion-button>
          </ion-item>
          <ion-item>
            <ion-img src="caballo.jpeg"></ion-img>
            <ion-label class="m-2 text-sm">
              <h2>Caballo</h2>
              <p>Hiiii hiiii</p>
            </ion-label>
            <ion-button slot="end" fill="outline" @click="playSound('caballo-sonido.mp3')">
              <play-button/>
            </ion-button>
          </ion-item>
          <ion-item>
            <ion-img src="burro.jpeg"></ion-img>
            <ion-label class="m-2 text-sm">
              <h2>Burro</h2>
              <p>Hiaaa hiaaa</p>
            </ion-label>
            <ion-button slot="end" fill="outline" @click="playSound('burro-sonido.mp3')">
              <play-button/>
            </ion-button>
          </ion-item>
          <ion-item>
            <ion-img src="conejo.jpg"></ion-img>
            <ion-label class="m-2 text-sm">
              <h2>Conejo</h2>
              <p>Cuix cuix</p>
            </ion-label>
            <ion-button slot="end" fill="outline" @click="playSound('conejo-sonido.m4a')">
              <play-button/>
            </ion-button>
          </ion-item>
        </ion-list>
      </div>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonContent, IonPage, IonButton, IonImg  } from '@ionic/vue';
import   playButton   from '../components/icons/playButton.vue';

function playSound(audioFile: string) {
  const audio = new Audio(audioFile);
  audio.play();
}
</script>

<style scoped>
ion-item{
  display: flex;
  justify-content: space-between;
}

ion-button{
  height: 50px;
  width: 50px;
}

ion-img {
  width: 200px;
  height: 200px;
}
</style>
