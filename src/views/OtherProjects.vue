<template>
  <main>
    <h1>Diseño UX/UI</h1>

    <p>
      Gracias al Curso en <strong>Diseño de Experiencia de Usuario</strong>, he realizado tres proyectos finales de aplicación,
      tanto móvil como web, siguiendo rigurosamente todos los pasos de aprendidos.
    </p>
    <ProjectsList v-bind:projects="projects" class="proyectslist"/>
  </main>
</template>

<style scoped>

p{
  margin-bottom: 40px;
}

.proyectslist {
  margin-bottom: 30px;
}

h1 {
  font-family: 'Fira Sans';
}

@media only screen and (max-width: 620px){

main {
  margin: 12px;
}

.proyectslist {
  margin-bottom: 650px;
}

}
</style>

<script lang="ts">
import Vue from "vue";
import ProjectsList from "@/components/ProjectsList.vue";
import otherProjectsData from "@/data/OtherProjectsData.ts";

export default Vue.extend({
  name: "OtherProjects",
  components: {
    ProjectsList,
  },
  data: function () {
    return {
      projects: otherProjectsData,
    };
  },
});
</script>
