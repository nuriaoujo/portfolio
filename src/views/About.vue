<template>
  <main style="margin-bottom: 80px;">
    <h1>Hola!</h1>

    <div class="photo">
      <img src="img/avatar_nunu.png" alt="Nuria Oujo img"/>
    </div>

    <section class="paragraph">
      <article>
        Soy <strong>Nuria Oujo</strong>, Desarrolladora Junior Full Stack y Diseñadora UX/UI.<br/>
      </article>

      <article class="actual-position-art">Actualmente colaboro activamente en la gestión de redes del club de orientación
      <br/>
      <a href="https://www.instagram.com/adcarnela/" target="_blank">ADC Arnela</a> mientras me formo en <router-link to="/resume">Desarrollo Full Stack</router-link>.</article>

      <article class="actual-position-art">En estos momentos busco empleo como <strong>Desarrolladora Front End</strong>, 
      pero estoy abierta a explorar otras posibilidades laborales. Te invito a que nos mantengamos en contacto a través 
      de mi correo <a href="mailto:oujomiguez.nuria@gmail.com">oujomiguez.nuria@gmail.com</a> o pulsando el siguiente botón:</article>
    
      <div class="button-connect">
        <router-link class="router-link" to="/contact">
          Conectemos
          <span class="material-symbols-outlined">arrow_forward</span>
        </router-link>
        
      </div>
    </section>

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

.paragraph {
  max-width: 700px;
  margin-bottom: 20px;
}

.photo {
  float: right;
  margin-top: 3%;
  text-align: center;

  img {
    width: 200px
  }
}

.actual-position-art {
 margin-top: 30px;
}

@media only screen and (max-width: 620px){
  main {
    margin: 12px;
  }
  .paragraph {
    float: left;
  }

  .photo {
    width: 100%;
    margin-bottom: 7%
  }

  .button-connect {
    padding: 9px 70px 9px 70px;
  }
}

</style>