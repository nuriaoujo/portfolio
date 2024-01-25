<template>
  <main style="margin-bottom: 80px;">
    <h1>Hola!</h1>

    <div class="photo">
      <img src="img/avatar_nunu.png" alt="Nuria Oujo img"/>
    </div>

    <article>
      <p>
        Soy <span class="bold">Nuria Oujo</span>, Desarrolladora Junior Full Stack y Diseñadora UX/UI.
      </p>

      <p class="actual-position-art">
        Actualmente colaboro activamente en la gestión de redes del club de orientación
        <br>
        <a href="https://www.instagram.com/adcarnela/" target="_blank">ADC Arnela</a> 
        mientras me formo en <router-link to="/resume">Desarrollo Full Stack</router-link>.
      </p>

      <p class="actual-position-art">
      En estos momentos busco empleo como <span class="bold">Desarrolladora Front End</span>, 
      pero estoy abierta a explorar otras posibilidades laborales. Te invito a que nos mantengamos en contacto a través 
      de mi correo <a href="mailto:oujomiguez.nuria@gmail.com">oujomiguez.nuria@gmail.com</a> o pulsando el siguiente botón:
      </p>
    
      <div class="button-connect">
        <router-link class="router-link" to="/contact">
          Conectemos
          <span class="material-symbols-outlined">arrow_forward</span>
        </router-link>
        
      </div>
    </article>

    <div style="clear:both"></div>

  </main>
</template>

<style scoped>

h1 {
  font-family: 'Fira Sans';
}

.button-connect {
  margin-top: 30px;
  margin-right: 78%;
  padding: 9px;
  border: 1.5px solid #B7CADB;

  .router-link {
    display: flex;
    align-items: center;
    justify-content: space-around;
  }
}

.material-symbols-outlined {
  display: inline-block;
}

article{
  max-width: 700px;
  margin-bottom: 20px;
}

.photo {
  float: right;
  margin-top: 3%;
  text-align: center;

  img {
    width: 200px;
  }
}

.bold {
  font-weight: bold;
}

.actual-position-art {
 margin-top: 30px;
}

@media only screen and (max-width: 620px){
  main {
    margin: 12px;
  }

  article {
    float: left;
  }

  .photo {
    width: 100%;
    margin-bottom: 7%;

    img {
      width: 170px;
    }

  }

  .button-connect {
    padding: 9px 70px 9px 70px;
  }
}

</style>