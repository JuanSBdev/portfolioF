
<script setup>
import { i18n } from '../main'

const redireccionarCalculadora = () => {
  window.open("https://venerable-choux-eccf3d.netlify.app/");
};
const redireccionarCarta = () => {
  window.open("https://juansbdev.github.io/carta/");
};
const redireccionarApi = () => {
  window.open("https://beamish-trifle-472703.netlify.app/");
};
const redireccionarLista = () => {
  window.open("https://juansbdev.github.io/listaDeTareas/");
};
const redireccionarCoder = () => {
  window.open("https://kira-mobile-9vh6gn.flutterflow.app/");
};


</script>
<template>
    <div  v-if="i18n.global.locale === 'es'" class="contenedor-pro">
        <h5 class="h3-con">
            { Mis proyectos }
        </h5>
        <div class="wraper sobra">
            
            <div
            @click="redireccionarCarta"
            class="carta col-6 col-sm-2 card">
            <img src="https://juansbdev.github.io/carta/img/logo2-removebg-preview.png" alt="Logo ">
            <h6> Menu Mobile</h6>
            <p> Se utiliza para esta mobile app html5 - css3 - bootstrap - javascript</p>
        </div>
        <div
            @click="redireccionarCoder"
            class="kira col-6 col-sm-2 card">
            <img src="https://kirasystems.com/files/press-kit/logos/Kira-logo_WEB.png" alt="Logo Kirá ">
               <h6>Rental App</h6>
               <p>App de alquileres , multiplataforma, desarrollada en Flutterflow, dart, firebase</p> 
            </div>
        <div @click="redireccionarCalculadora" class="calculadora col-6 col-sm-2  card">
                
            
            <img src="https://cdn-icons-png.flaticon.com/512/4564/4564300.png" alt=" logo">
            <h6>e-commerce</h6>
                <p>React.js, JavaScript, HTML5, CSS3, Redux, Bootstrap, Express.JS, PostgreSQL, Sequelize, MercadoPago JWT, Auth0, firebase</p>
        </div>
        <div
        @click="redireccionarApi"
        class="api col-6 col-sm-2 card">
        <img src="https://fairbanksmuseum.org/wp-content/uploads/2023/03/partly_sunny.png" alt="logo">
        <h6>Clima API</h6>
        <p>App desarrollada en React.js - utilizando HTML5 - CSS - SASS - API REST - DEPLOYED</p>
    </div>
    <div
            @click="redireccionarLista"
             class="lista col-6 col-sm-2 card">
             <img src="https://cdn-icons-png.flaticon.com/512/6194/6194029.png" alt="logo">
             <h6>To Do List.</h6>
                <p>App desarrollada utilizando JavaScript Vanilla, HTML 5 Y CSS - DEPLOYED</p>

            </div>
        </div>
    </div>

    <div  v-else class="contenedor-pro">
        <h5 class="h3-con">
            { Some Projects }
        </h5>
        <div class="wraper sobra">
            
            
            <div
             @click="redireccionarCarta"
             class="carta col-6 col-sm-2 card">
             <img src="https://juansbdev.github.io/carta/img/logo2-removebg-preview.png" alt="logo">
             <h6> Menu Mobile Foodtruck</h6>
                <p> Freelance job - mobile app developed with html5 - css3 - bootstrap - javascript</p>
            </div>
            <div
            @click="redireccionarCoder"
            class="kira col-6 col-sm-2 card">
            <img src="https://kirasystems.com/files/press-kit/logos/Kira-logo_WEB.png" alt="Logo Kirá ">
               <h6>Rental App</h6>
               <p>Rental App, multiplataforma, developed with Flutterflow, firebase, dart</p> 
            </div>

            <div @click="redireccionarCalculadora" class="calculadora col-6 col-sm-2  card">
                <img src="https://cdn-icons-png.flaticon.com/512/4564/4564300.png" alt="logo">
                <h6>e-Commerce</h6>
                <p>React.js, JavaScript, HTML5, CSS3, Redux, Bootstrap, Express.JS, PostgreSQL, Sequelize, MercadoPago JWT, Auth0, firebase</p>
        </div>
        
            <div
            @click="redireccionarApi"
             class="api col-6 col-sm-2 card">
             <img src="https://fairbanksmuseum.org/wp-content/uploads/2023/03/partly_sunny.png" alt="logo">
             <h6>Weather API</h6>
                <p>App developed with React.js - using HTML5 - CSS - SASS - API REST - DEPLOYED</p>
            </div>
            <div
            @click="redireccionarLista"
             class="lista col-6 col-sm-2 card">
             <img src="https://cdn-icons-png.flaticon.com/512/6194/6194029.png" alt="logo">
             <h6>To Do List.</h6>
                <p>App developed with Vanilla JavaScript, localstorage, HTML 5 Y CSS - DEPLOYED</p>

            </div>
        </div>
    </div>
    
</template>
<style scoped>
@media screen and (max-width: 574px) {

    .h3-con{
        font-family: 'Ubuntu', sans-serif;

        color: rgb(247, 186, 247);
    }
    h5{
        font-size: 4rem;
        display: flex;
        justify-content: center;
        margin-top: 6rem;
    }
    img{
        width: 60%;
    }
    .wraper{
        width: 100%;
        padding-top: 3rem;
        display: flex;
        flex-flow: row-reverse wrap;
        align-items: center;
        justify-content: space-evenly;
        } 
    .card{
        width: 40%;
        padding: 2%;
        min-height: 250px;
        background-color: rgba(238, 130, 238, 0);
        border: none;
    }
    .card h6{
        font-size: 2rem;
        color: rgb(247, 186, 247);
        font-family: 'Ubuntu', sans-serif;
    }
    .card p{
        font-size: 1rem;
        color: rgb(247, 186, 247);
        font-family: 'Ubuntu', sans-serif;
    }
    .kira img{
        margin: 30% 0 30%  0 ;
    }
    .carta img{
        width: 40% ;
    }
}
@media screen and (min-width: 575px) and (max-width:768px) {
    .h3-con{
        font-family: 'Ubuntu', sans-serif;

        color: rgb(237, 56, 243);
        font-size: 4rem;
        display: flex;
        justify-content: center;
        margin-top: 6rem;
    }
   
    
    img{
        width: 20%;
        min-width: 150px;
        max-width: 200px;
    }
    .contenedor-pro{
        display: flex;
        flex-flow: column nowrap;
        align-items: center;
    }
    .wraper{
        width: 80%;
        padding-top: 5%;
        display: flex;
        flex-flow: row-reverse wrap;
        align-items: stretch;
        justify-content: space-evenly;
        color: rgb(241, 215, 241);
        } 
    .card{
        display: flex;
        flex-wrap: nowrap;
        width: 40%;
        padding: 2%;
        
        background-color: rgba(238, 130, 238, 0);
        border: none;
        font-family: 'Ubuntu', sans-serif;

    }
    .card h6{
     
        font-size: 2rem;
    }
    .kira img{
        margin: 30% 0 20% 0 ;
    }
    .carta img{
        width: 40% ;
    }

}
@media screen and (min-width: 769px) {
    
    h5{
        font-size: 4rem;
        display: flex;
        justify-content: center;
        margin-top: 6rem;
    }
    h6{
        font-size: 1.5rem;
    }
   
    img{
        width: 60%;
    }
    
    .contenedor-pro{
        margin-right: 1%;
    }
    .wraper{
        width: 90%;
        margin: 5%;

        display: flex;
        text-align: center;
        align-items: stretch;
        align-content: center;

   
    }
    .h3-con{
        color: rgb(247, 186, 247);
        font-family: 'Ubuntu', sans-serif;


    }
    .card{
        text-decoration: none;
        border-radius: 1rem;
        box-shadow: 0 0 10px 0 rgb(50, 12, 70);
        background-color: rgb(246, 230, 246);
        padding: 2%;
        margin: 2%;
        padding-bottom: 0%;
        min-height: 200px;

        display: flex;
        flex-flow: column nowrap;
        align-items: center;
        justify-content: space-between;
        color: rgb(66, 54, 72);
    }

    .card:hover{
        transform: scale(1.1);
    }

    .card h6, p {
        background-image: linear-gradient(45deg,#4a2d89 0%,#ac43cc 35%,#411f8b 85%,#6c3870 100%);
        -webkit-text-fill-color: transparent;
        -webkit-background-clip: text;  
    }
    .card p{
        display: flex;
        align-items: center;
        height: 100%;
        font-size: .8rem; 
    }

    .card img{
        margin: 4%;
    }

    .carta img{
        margin-top: -5%;
        width: 90%;
    }
    .kira img{
        margin: 30% 30% ;
    }
a{
    text-decoration: none;
    
}

}
</style>
