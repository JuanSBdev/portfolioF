<script setup>
import {i18n} from '../main'
let verCertHenry = ()=>{
    window.open("https://certificates.soyhenry.com/new-cert?id=f65faf2e725ec6df6adfa805a01aa29945534edfb1bf8ec84070219fe31ab5d7")
}
const verCertNuclea = () => {
  window.open("https://www.linkedin.com/feed/update/urn:li:activity:7171272554777591811/");
};
const verCertCoderhouse = () => {
  window.open("https://i.ibb.co/c3HF8N1/coder-cert.png");
};
</script>
<template>
<div class="cont mt-5 pt-5">

    <h2 v-if="i18n.global.locale=== 'es'" > ¿Donde me capacito?</h2>
    <h2 v-else > Learning Hub</h2>
    <div class="containerDonde">

        <div v-if="i18n.global.locale=== 'es'"  class="wraper">
            <div  class="soy col-sm-3">
                <h3> Soy Henry </h3>
                <p> JavaScript (avanzado) , estructura de datos, React.js, Redux, Node.js, Express, SQL, PostgreSQL, Sequelize, Figma y más...</p>
                <img  @click="verCertHenry"  src="https://i.ibb.co/zmxgxnq/certificado-henry-page-0001.jpg" alt="Certificate Henry">
                
            </div>
            <div class="udemy  col-sm-3 ">
                <h3>Nuclea</h3>
                <p class="mb-12" >Donde aprendo y trabajo con Flutterflow, firebase y dart además de diseño mobile y flutter.</p>
                <img @click="verCertNuclea" src="../assets/resources/cert.jpeg" alt="constancia nuclea">
                
            </div>
            <div  class="coder  col-sm-3 items-center justify-center ">
                <h3> Coderhouse</h3>
                <p class="mb-10">Html5, css3, bootstrap, Sass, github, git, SEO, subida al servidor, clientes y presupuestos.</p>
                <img  @click="verCertCoderhouse" src="https://i.ibb.co/c3HF8N1/coder-cert.png" alt="Certificate CoderHouse">
            </div>
            
        </div>
        <div v-else class="wraper row">
            <div class="soy col-sm-3">
    <h3>Soy Henry</h3>
    <p>Advanced JavaScript, data structures, React, Redux, Node.js, Express, SQL, PostgreSQL, Sequelize, Figma & more.</p>
    <img @click="verCertHenry" src="https://i.ibb.co/zmxgxnq/certificado-henry-page-0001.jpg" alt="Certificate SoyHenry">
            
</div>
<div class="udemy col-sm-3">
    <h3>Nuclea</h3>
    <p class="mb-12">Where I learn and work with FlutterFlow, Firebase, and Dart, as well as mobile design and Flutter.</p>
    <img  @click="verCertNuclea" src="https://media.licdn.com/dms/image/D4D22AQEpd9bVkMUw6g/feedshare-shrink_2048_1536/0/1709764611638?e=1713398400&v=beta&t=N66w0eHgnLBIQA6-fu3laQvpjW48uvGK-Gwrh6mRf1E" alt="constancia nuclea">
            
</div>
<div  class="coder col-sm-3 ">
    <h3>Coderhouse</h3>
    <p class="mb-10">HTML5, CSS3, Bootstrap, Sass, GitHub, Git, SEO, FileZilla,  server deployment, clients, and budgets.</p>
    <img @click="verCertCoderhouse" src="https://i.ibb.co/c3HF8N1/coder-cert.png" alt="">
    
</div>


        </div>
    </div>
</div>
</template>
<style scoped>
@media screen and (max-width: 574px) {
    img{
        width: 40%;
        margin-bottom: 12%;
    }
    p{
        width: 80%;
    }
    h2{
        font-size: 2rem;
        width: 100%;
        display: flex;
        justify-content: center;
        padding: 4rem;
    }
    #p2 {
        color: rgba(14, 11, 11, 0.295);
        padding: 5%;
        margin-bottom: 0% ;
        padding-top: .8rem;
        text-decoration: none;
        font-size: 1.2rem;
    }
    .containerDonde{
        display: flex;
        justify-content: center;
        margin-top: 1%;
        width: 100%;
        color: aliceblue;
        font-family: 'Ubuntu', sans-serif;
        
    }
    .wraper{
        width: 90%;
        margin-left: 5%;
        margin-right: 0%;
        display: flex;
        flex-flow: row-reverse wrap;
        justify-content: space-evenly;
        align-items:start;
        text-align: center;
        
    }

    .ver{
        display:flex;
        margin-left: 30%;
        justify-content: center;
        width: 40%;
        position:relative;
        bottom: 8rem;
        border-radius: 1rem;
        background-color: rgba(119, 61, 184, 0.37);
        box-shadow: 5px 5px 5px black;
    }
    
}
@media screen and ( max-width: 1023px) {
    img{
        width: 100%;
        margin-top: 12%;
    }
    h2{
        font-size: 2rem;
        width: 100%;
        display: flex;
        justify-content: center;
        padding: 4rem;
        color: aliceblue;
    }
    #p2 {
        display: none;
    }
    .containerDonde{
        display: flex;
        justify-content: center;
        margin-top: 1%;
        width: 100%;
        margin-bottom: 20%;
        color: aliceblue;
        font-family: 'Ubuntu', sans-serif;
        
    }
    .wraper{
        width: 90%;
        margin-left: 5%;
        margin-right: 0%;
        display: flex;
        flex-flow: row-reverse wrap;
        justify-content: space-evenly;
        align-items:start;
        text-align: center;
        
    }
    
    :hover.coder img{
        filter: blur(1px);
        
    }
    .ver{
        display:flex;
        margin-left: 30%;
        justify-content: center;
        width: 40%;
        position:relative;
        bottom: 8rem;
        border-radius: 1rem;
        background-color: rgba(119, 61, 184, 0.37);
        box-shadow: 5px 5px 5px black;
    }
}

@media screen and (min-width: 1024px) {
    
    .containerDonde{
        display: flex;
        justify-content: center;
        color: aliceblue;
        font-family: 'Ubuntu', sans-serif;
    }
    h2{

        color: aliceblue;
        width: 100%;
        display: flex;
    justify-content: center;
    padding: 5rem;
}

.wraper{
    width: 80%;
    display: flex;
    flex-flow: row-reverse wrap;
    align-items:start;
    align-content: stretch;
    justify-content: space-around;

}

.coder img{
    width:100%;
    padding: 0%;
}
.coder img:hover{
    transform: scale(1.1);
    
}
.ver{
        display:flex;
        margin-left: 20%;
        justify-content: center;
        width: 60%;
        position:relative;
        bottom: 8rem;
        border-radius: 1rem;
        background-color: rgba(118, 61, 184, 0.034);
        padding: rem;
        box-shadow: 5px 5px 5px black;
    }
    :hover.ver{
        background-color: rgba(236, 240, 9, 0.39);
    }

 #p2 {
    z-index: 10;
        color: rgba(14, 11, 11, 0.295);
        padding: 5%;
        margin-bottom: 0% ;
        padding-top: .8rem;
        font-size: 1.2rem;
    }
    :hover#p2{
        color: black;
    }
    .coder a{
        text-decoration: none;
        
}
.soy{
    display: flex;
    flex-direction: column;
    align-items: start;
}
.soy img{
    display: flex;
    align-self: center;
    width: 100%;
 
}
.soy img:hover{
   transform: scale(1.1);
   
 
}
.udemy img{
    width:100%;

}
.udemy img:hover{
    transform: scale(1.1);
}
}
</style>