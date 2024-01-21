<template>
  <div>
    <h1>Perfil</h1>

    <div class="paragraph">
      <div class="main-txt">Soy <strong>Nuria Oujo</strong>,</div> Desarrolladora Junior Full Stack y Diseñadora UX/UI.
      <br/>
      <br/>
      Con una formación inicial en <strong>Bellas Artes</strong>, mi trayectoria ha evolucionado hacia el ámbito tecnológico,
      destacando mi especialización en <strong>Diseño de Experiencia de Usuario</strong> (UX) mediante un curso de Google.
      Impulsada por el deseo de ampliar mis conocimientos, me sumergí en el desarrollo Frontend a través de Campus Dual TIC, 
      culminando en la exitosa conclusión de un <strong>Bootcamp en Desarrollo Full Stack</strong>.
      <br/>
      <br/>
      Mi enfoque multidisciplinario y mi capacidad para integrar creatividad y habilidades técnicas me posicionan como una candidata polivalente, 
      lista para afrontar nuevos desafíos y seguir formándome como programadora Full Stack.
      <br/>
      <br/>
      Gracias por valorar mi perfil, os invito a que 
      <router-link to="/contact">conectéis conmigo</router-link>.

      <div style="margin-top:20px; margin-bottom:20px;">
        <a class="download-link" href="d/nuriaoujo_cv.pdf" target="_blank"><i class="fa fa-download fa-lg fa-fw"></i> Descarga mi CV</a>
        <div style="clear:both"></div>
      </div>
    </div>
    <div class="photo">
      <img src="img/avatar_nunu.png" alt="Nuria Oujo img" />
    </div>

    <div style="clear:both"></div>

    <hr>

    <div class="full-content">

      <h2>Estudios</h2>

      <h3>Bootcamp en Desarrollo Full Stack</h3>
      <h4>CampusDualTIC</h4>
      <div>08/2023 - 11/2023 | Remoto</div>

      <h3>Bootcamp en Introducción a la Programación</h3>
      <h4>CampusDualTIC</h4>
      <div>03/2023 - 06/2023 | Remoto</div>

      <h3>Máster en Cine, Comunicación e Industria Audiovisual</h3>
      <h4>Universidad de Valladolid</h4>
      <div>2021 - 2022 | Valladolid, España</div>

      <h3>Grado en Bellas Artes</h3>
      <h4>Universidad de Vigo</h4>
      <div>2017 - 2021 | Pontevedra, España</div>

      <h2>Experiencia profesional</h2>

      <h3>Bootcamp en Desarrollo Full Stack</h3>
      <h4>CampusDualTIC</h4>
      <div>08/2023 - 11/2023 | Remoto</div>
      <div class="tech-stack">Angular , JavaScript, PostgreSQL, Spring, Java</div>

      <h3>Bootcamp en Introducción a la Programación</h3>
      <h4>CampusDualTIC</h4>
      <div>03/2023 - 06/2023 | Remoto</div>
      <div class="tech-stack">Angular , JavaScript, SQL, Spring, Java</div>

      <h2>Cursos</h2>

      <h3>JavaScript Moderno: Guía para dominar el lenguaje</h3>
      <h4>dev/talles</h4>
      <div>01/2024</div>

      <h3>Diseño de Experiencia del Usuario (UX) de Google</h3>
      <h4>Coursera</h4>
      <div>10/2022 - 06/2023</div>

      <h3>Modern HTML & CSS From The Beginning (Including Sass)</h3>
      <h4>Udemy</h4>
      <div>06/2022</div>


      <h2>Conocimientos</h2>

      <div class="skill-set">
        <h3>Desarrollo Full Stack </h3>
        <SkillRate name="TypeScript" :rate="4" />
        <SkillRate name="HTML5" :rate="4" />
        <SkillRate name="CSS3" :rate="4" />
        <SkillRate name="Angular" :rate="3" />
        <SkillRate name="Spring" :rate="3" />
        <SkillRate name="Java" :rate="3" />
        <SkillRate name="PostreSQL" :rate="3" />
      </div>

      <div class="skill-set">
        <h3>Diseño UX/UI</h3>
        <SkillRate name="Figma" :rate="4" />
        <SkillRate name="InDesign" :rate="4" />
        <SkillRate name="Photoshop" :rate="5" />
        <SkillRate name="Illustrator" :rate="4" />
        <SkillRate name="Adobe XD" :rate="3" />
      </div>
      <div style="clear:both" />

      <h2>Idiomas</h2>

      <h3>Castellano</h3>
      <div>Competencia bilingüe o nativa</div>

      <h3>Gallego</h3>
      <div>Competencia bilingüe o nativa</div>

      <h3>Inglés</h3>
      <div>Competencia básica profesional</div>


    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import SkillRate from "@/components/SkillRate.vue";

export default Vue.extend({
  name: "Resume",
  components: {
    SkillRate,
  },
});
</script>

<style scoped>
h2 {
  font-weight: 100;
  font-size: 2em;
  margin: 0px;
  padding: 0px;
  padding-top: 50px;
}
h3 {
  font-weight: 100;
  font-size: 1.6em;
  margin: 0px;
  padding: 0px;
  padding-top: 30px;
}
h4 {
  font-weight: 100;
  font-size: 1.3em;
  margin: 0px;
  padding: 0px;
  padding-top: 15px;
  font-style: italic;
}

.paragraph {
  max-width: 700px;
}

.main-txt {
  font-size: 1.50rem;
}

.download-link {
  float:left;
  margin-right: 50px;
}

.full-content div {
  max-width: 800px;
}

.skill-set h3 {
  padding-bottom: 10px;
}

.photo img {
  height: 300px;
  width: 300px;
}

.tech-stack {
  font-style: italic;
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
    padding: 30px;
    padding-left: 80px;
  }

  .skill-set {
    float: left;
    padding-right: 60px; 
  }
}
</style>