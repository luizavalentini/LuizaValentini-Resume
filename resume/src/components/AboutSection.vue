<template>
    <section id="about">
      <p class="section__text__p1">Get To Know More</p>
      <h1 class="title">About Me</h1>
      <div class="section-container">
        <div class="section__pic-container">
          <img
            src="../assets/about-pic.jpg"
            alt="Profile picture"
            class="about-pic"
          />
        </div>
        <div class="about-details-container">
          <div class="about-containers">
            <div class="details-container">
              <img
                src="../assets/experience.png"
                alt="Experience icon"
                class="icon"
              />
              <h3>Experience</h3>
              <p>Frontend development</p>
              <p>Mobile Development</p>
            </div>
            <div class="details-container">
              <img
                src="../assets/education.png"
                alt="Education icon"
                class="icon"
              />
              <h3>Education</h3>
              <p>
                Software Engineering Bachelors Degree – Conclusion: 2024/2<br />Pontifical
                Catholic University of Rio Grande do Sul (PUCRS)
              </p>
            </div>
          </div>
          <div class="text-container">
            <p class="about-me-text">
              Student of the sixth semester from the course of Software
              Engineering from the Pontifical Catholic University of Rio Grande do
              Sul. After the past years I started to be very interested in
              frontend and mobile development, not just by usual purposes, but also for the
              innovation prospects, that help to make a difference in the world. I
              recognize the necessity to be always learning, and I’m open to do
              that everyday. My profile, is of someone creative, persistent and
              curious.
            </p>
          </div>
        </div>
      </div>
      <img
        src="../assets/arrow.png"
        alt="Arrow icon"
        class="icon arrow"
        onclick="location.href='./#experience'"
      />
    </section>
  </template>
  <script>
  export default {
    name: "AboutSection",
  };
  </script>
  <style>
  
  #about {
    position: relative;
  }
  
  .about-containers {
    gap: 2rem;
    margin-bottom: 2rem;
    margin-top: 2rem;
  }
  
  .about-details-container {
    justify-content: center;
    flex-direction: column;
  }
  
  .about-containers,
  .about-details-container {
    display: flex;
  }
  
  .about-pic {
    border-radius: 2rem;
  }
  
  .arrow {
    position: absolute;
    right: -5rem;
    bottom: 2.5rem;
  }
  
  .details-container {
    padding: 1.5rem;
    flex: 1;
    background: white;
    border-radius: 2rem;
    border: rgb(53, 53, 53) 0.1rem solid;
    border-color: rgb(163, 163, 163);
    text-align: center;
  }
  
  .section-container {
    gap: 4rem;
    height: 80%;
  }
  
  .section__pic-container {
    height: 400px;
    width: 400px;
    margin: auto 0;
  }
  .about-me-text{
    text-align: justify;
  }
  </style>