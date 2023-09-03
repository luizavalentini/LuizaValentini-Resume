<template>
  <section id="profile">
    <div class="section__pic-container">
      <div></div>
      <img class="profile-picture" src="../assets/profile-picture.jpg" />
    </div>
    <div class="section__text">
      <p class="section__text__p1">Hello, I'm</p>
      <h1 class="title">Luiza Valentini</h1>
      <p class="section__text__p2">Frontend Developer</p>
      <div class="btn-container">
          <button
          class="btn btn-color-2"
        >
          Download CV
        </button>
        <button class="btn btn-color-1" >
          Contact Info
        </button>
      </div>
      <div id="socials-container">
        <img
          src="../assets/linkedin.png"
          alt="My LinkedIn profile"
          class="icon"
          @click="openLink('https://www.linkedin.com/in/luizavalentini/')"
        />
        <img
          src="../assets/github.png"
          alt="My Github profile"
          class="icon"
          @click="openLink('https://github.com/luizavalentini')"
        />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ProfileSection",
  methods: {
    openLink(url) {
      window.open(url);
    },
   redirectToContact() {
      window.location.href = "#contact";
},
  },
};
</script>
<style>
section {
  padding-top: 4vh;
  height: 96vh;
  margin: 0 10rem;
  box-sizing: border-box;
  min-height: fit-content;
}

.section-container {
  display: flex;
}

#profile {
  display: flex;
  justify-content: center;
  gap: 5rem;
  height: 80vh;
}

.profile-picture {
  border-radius: 300px;
  width: 100%;
  height: 100%;
}

.section__pic-container {
  display: flex;
  height: 400px;
  width: 400px;
  margin: auto 0;
}

.section__text {
  align-self: center;
  text-align: center;
}

.section__text p {
  font-weight: 600;
}

.section__text__p1 {
  text-align: center;
}

.section__text__p2 {
  font-size: 1.75rem;
  margin-bottom: 1rem;
}

.title {
  font-size: 3rem;
  text-align: center;
}

#socials-container {
  display: flex;
  justify-content: center;
  margin-top: 1rem;
  gap: 1rem;
}

/* ICONS */

.icon {
  cursor: pointer;
  height: 2rem;
}

/* BUTTONS */

.btn-container {
  display: flex;
  justify-content: center;
  gap: 1rem;
}

.btn {
  font-weight: 600;
  transition: all 300ms ease;
  padding: 1rem;
  width: 8rem;
  border-radius: 2rem;
}

.btn-color-1,
.btn-color-2 {
  border: rgb(53, 53, 53) 0.1rem solid;
}

.btn-color-1:hover,
.btn-color-2:hover {
  cursor: pointer;
}

.btn-color-1,
.btn-color-2:hover {
  background: rgb(53, 53, 53);
  color: white;
}

.btn-color-1:hover {
  background: rgb(0, 0, 0);
}

.btn-color-2 {
  background: none;
}

.btn-color-2:hover {
  border: rgb(255, 255, 255) 0.1rem solid;
}

.btn-container {
  gap: 1rem;
}
</style>

