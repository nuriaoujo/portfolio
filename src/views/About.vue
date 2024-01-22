<template>
  <div style="margin-bottom: 80px;">
    <h1>Hola!</h1>

    <div class="paragraph">
      <div>
        Soy <strong>Nuria Oujo</strong>, Desarrolladora Junior Full Stack y Diseñadora UX/UI.<br/>
      </div>

      <div style="margin-top: 20px;">Actualmente colaboro activamente en la gestión de redes del club de orientación
      <br/>
      <a href="https://www.instagram.com/adcarnela/" target="_blank">ADC Arnela</a> mientras me formo en <router-link to="/resume">Desarrollo Full Stack</router-link>.</div>

      <div style="margin-top: 40px;">En estos momentos busco empleo como <strong>Desarrolladora Front End</strong>, 
      pero estoy abierta a explorar otras posibilidades laborales. Te invito a que nos mantengamos en contacto a través 
      de mi correo <a href="mailto:oujomiguez.nuria@gmail.com">oujomiguez.nuria@gmail.com</a> o pulsando el siguiente botón:</div>
    
      <div class="button-connect">
        <router-link class="router-link" to="/contact">
          Conectemos
          <span class="material-symbols-outlined">arrow_forward</span>
        </router-link>
        
      </div>
    </div>

    <div class="photo">
      <img src="img/avatar_nunu.png" alt="Nuria Oujo img" style="width: 200px" />
    </div>

    <div style="clear:both"></div>

  </div>
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
  margin-top: 50px;
  text-align: center;
}

@media only screen and (min-width: 620px){
  .paragraph {
    float: left;
  }

  .photo {
    float: left;
    padding: 10px;
    padding-left: 80px;
  }
}

</style>