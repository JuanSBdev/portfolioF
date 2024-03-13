<script setup>
import { reactive } from 'vue';
import { useRouter } from 'vue-router';
import { i18n } from './main.js';
import { RouterLink, RouterView } from 'vue-router';
const btnImgEs = 'https://www.debate.com.mx/__export/1655135059914/sites/debate/img/2022/06/13/bandera_de_argentina-_qux_significa-2_1.jpg_423682103.jpg';
const btnImgEn = 'https://media.istockphoto.com/id/1211686337/es/vector/bandera-del-reino-unido-bandera-del-reino-unido.jpg?s=612x612&w=0&k=20&c=PLg6ZYHXGQBQrou38WRg2fnvKGAaGh3iblsna-11qd0=';
function changeLanguage() {
  i18n.global.locale = i18n.global.locale === 'es' ? 'en' : 'es';
  };
// const router = useRouter();

</script>

<template>
  <head>
    
    <link rel="shortcut icon" href="https://cdn-icons-png.flaticon.com/512/2534/2534928.png" type="image/x-icon">
  </head>
  
  <main > 
    <div class="language">
     
      <button class="btn-lang" @click="changeLanguage">  
        <p  v-if="i18n.global.locale=== 'es'"  class="bandera" >En</p>
        <p v-else  class="bandera">Es</p>
      </button>
    </div>
    <router-view></router-view>
  </main>
</template>

<style>
@import "./assets/base.css";



.language{
  z-index: 3;
  position:absolute;
  right: 2%;
  top: 5PX;
  width: 40px;
  
  overflow: hidden;
}
.btn-lang{
  width: 100%;
}
.bandera{
  display: flex;
  justify-content: center;
  font-size: 1.4rem;
  color: aliceblue;
  font-family:Arial, Helvetica, sans-serif;
  border-radius: 10rem;
}
@media screen and (max-width: 640px) {
  .language{
  z-index: 3;
  position:absolute;
  right: 8%;
  top: 45PX;
  width: 30px;
  
  overflow: hidden;
}
  .bandera{
  display: flex;
  justify-content: center;
  font-size: 1.4rem;
  font-family:Arial, Helvetica, sans-serif;

}
}
</style>
