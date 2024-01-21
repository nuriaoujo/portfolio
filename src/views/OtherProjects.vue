<template>
  <div>
    <h1>Diseño UX/UI</h1>

    <div style="margin-bottom: 30px;">
      Gracias al Curso en <strong>Diseño de Experiencia de Usuario</strong>, he realizado tres proyectos finales de aplicación,
      <br/>
      tanto móvil como web, siguiendo rigurosamente todos los pasos de aprendidos.
      <br/>
      <br/>

    </div>
    <ProjectsList v-bind:projects="projects" />
    <br/>
  </div>
</template>

<style scoped>

h1 {
  font-family: 'Fira Sans';
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
