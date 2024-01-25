<template>
  <main>
    <h1>Desarrollo Full Stack</h1>

    <p>
      Actualmente me estoy formando como <span>Desarrolladora Full Stack</span>.
      <br/>
      Estos son algunos de los proyectos que he finalizado durante estos últimos meses.
    </p>

    <ProjectsList v-bind:projects="projects" class="proyects-margin" />

    <p class="near-footer">
      Puedes visualizar mi progreso en <a target="_blank" href="https://github.com/nuriaoujo">GitHub</a>.
    </p>
  </main>
</template>

<style scoped>

.proyects-margin {
  margin-bottom: 17%;
}

h1 {
  font-family: 'Fira Sans';
}

p {
  margin-bottom: 30px;
  margin-top: 20px;
}

span {
  font-weight: bold;
}

@media only screen and (max-width: 620px){
  main {
    padding: 12px;
  }

  .near-footer {
    margin-top: 1250px;
  }
}

</style>

<script lang="ts">
import Vue from "vue";
import ProjectsList from "@/components/ProjectsList.vue";
import gameProjectsData from "@/data/GameProjectsData.ts";

export default Vue.extend({
  name: "GameProjects",
  components: {
    ProjectsList
  },
  data: function () {
    return {
      projects: gameProjectsData,
    };
  },
});
</script>
