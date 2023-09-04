<template>
  <section id="projects">
    <p class="section__text__p1">Browse My Recent</p>
    <h1 class="title">Projects</h1>
    <div class="experience-details-container">
      <div class="about-containers">
        <div class="details-container color-container">
          <div class="article-container">
            <img
              src="../assets/enadeapp.png"
              alt="Project 1"
              class="project-img"
            />
          </div>
          <h2 class="experience-sub-title project-title">EnadeApp</h2>
          <div class="btn-container">
            <button
              class="btn btn-color-2 project-btn"
              @click="openLink('https://petinfpucrs.github.io/') "
            >
            Wiki Page
            </button>
          </div>
        </div>
        <div class="details-container color-container">
          <div class="article-container">
            <img
              src="../assets/denunciaaviolencia.png"
              alt="Project 2"
              class="project-img"
            />
          </div>
             <h2 class="experience-sub-title project-title">Denúncia a Violência</h2>
          <div class="btn-container">
            <button
              class="btn btn-color-2 project-btn"
              @click="openLink('https://tools.ages.pucrs.br/denuncia-a-violencia/denuncia-a-violencia-wiki/-/wikis/home') "
            >
              Wiki Page
            </button>
          </div>
        </div>
        <div class="details-container color-container">
          <div class="article-container">
            <img
              src="../assets/project-idoso+.png"
              alt="Project 3"
              class="project-img"
            />
          </div>
          <h2 class="experience-sub-title project-title">Idoso +</h2>
          <div class="btn-container">
            <button
              class="btn btn-color-2 project-btn"
              @click="openLink('https://tools.ages.pucrs.br/idoso-mais/idoso-mais-wiki/-/wikis/home') "
            >
            Wiki Page
            </button>
          </div>
        </div>
      </div>
      </div>
    <img
      src="../assets/arrow.png"
      alt="Arrow icon"
      class="icon arrow"
      onclick="location.href='./#contact'"
    />
  </section>
</template>
<script>
export default {
  name: "ProjectsSection",
  methods: {
    openLink(url) {
      window.open(url);
    },
}
};
</script>
<style>
#projects {
  position: relative;
}

.color-container {
  border-color: rgb(163, 163, 163);
  background: rgb(250, 250, 250);
}

.project-img {
  border-radius: 2rem;
  width: 90%;
  height: 90%;
}

.project-title {
  font-size: small;
  margin: 1rem;
  color: black;
}

.project-btn {
  color: black;
  border-color: rgb(163, 163, 163);
}

</style>