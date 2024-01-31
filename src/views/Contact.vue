<template>
  <main>
    
    <h1>¡Conectemos!</h1>

    <article>
      <p>Actualmente <strong>estoy buscando empleo</strong>,</p>
      <p>
        Estoy explorando nuevas oportunidades profesionales y me encantaría formar parte de vuestro equipo.
        Si considerais que mi perfil puede contribuir a vuestros proyectos... ¡No dudéis en contactar conmigo!
      </p>
      <p>
        ¡Gracias por visitar mi portfolio!
      </p>
      
    </article>

    <ul>
      <li>
        <i class="fa fa-envelope-o fa-lg fa-fw icon"></i>
        <a href="mailto:oujomiguez.nuria@gmail.com" target="_blank">oujomiguez.nuria@gmail.com</a>
      </li>
      <li>
        <i class="fa fa-linkedin fa-lg fa-fw icon" style="vertical-align: -5%;"></i>
        <a href="https://www.linkedin.com/in/nuriaoujo/" target="_blank">linkedin.com/in/nuriaoujo/</a>
      </li>
      <li>
        <i class="fa fa-github fa-lg fa-fw icon"></i>
        <a href="https://github.com/nuriaoujo" target="_blank">github.com/nuriaoujo</a>
      </li>
    </ul>

  </main>
</template>

<style scoped>

article {
  margin-bottom:40px;
}

h1 {
  font-family: 'Fira Sans';
}

ul {
  list-style: none;
  padding-inline-start: 0px;
}

li {
    line-height: 1.8em;
    font-size: 1.2em;
  }

@media only screen and (max-width: 620px){
  main {
    margin: 12px;
  }

  .icon {
    weight:10px;
  }
}

@media only screen and (min-width: 620px){

  ul {
    padding-inline-start: 40px;
  }

  li {
    line-height: 2em;
    font-size: 1.4em;
  }
}

i {
  margin-right: 20px;
}
</style>
