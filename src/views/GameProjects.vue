<template>
  <div>
    <h1>Desarrollo Full Stack</h1>

    <div style="margin-bottom: 30px;">
      The following are some stuff I've made or heavily contributed to.
    </div>

    <ProjectsList v-bind:projects="projects" class="proyects-margin" />

    <div style="margin-top: 20px;">
      Puedes visualizar mi progreso en <a target="_blank" href="https://github.com/nuriaoujo">GitHub</a>.
    </div>
  </div>
</template>

<style scoped>

.proyects-margin {
  margin-bottom: 17%;
}

h1 {
  font-family: 'Fira Sans';
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
