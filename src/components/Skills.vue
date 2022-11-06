<template>
  <section id="skill">
    <div>
      <img src="./../assets/ahhh.webp" alt="ahhh anime expression" width="250" />
    </div>
    <div class="greeting">
      <h1>Hi, i'm Andika Nice to meet you!</h1>

      <div class="desc">
        <p>
          Programming Hobbyist Java, Kotlin, Javascript, and other over 3 years experience developing, testing, and
          maintaining personal project software. I'm quietly confident, naturally curious, and perpetually working on
          improving my skills on programming.
        </p>
      </div>
    </div>
    <div class="skillGrid">
      <div class="skill1">
        <div>
          <img src="../assets/back.png" width="50px" alt="Desktop icon with binaries number inside it" />
        </div>
        <div>
          <p>Website Developing</p>
          <p>
            <b>Languages</b>
          </p>
          <p>HTML, CSS, Javascript, Node JS</p>
          <p>
            <b> Frameworks </b>
          </p>
          <div>
            <p>React JS</p>
            <p>Vue JS</p>
          </div>
          <p>
            <b>Development Tools</b>
          </p>
          <div>
            <p>Visual Studio Code</p>
            <p>Visual Studio</p>
            <p>Github</p>
            <p>Git</p>
          </div>
        </div>
      </div>
      <div class="skill2">
        <div>
          <img src="../assets/error.png" width="50px" alt="Desktop icon with error popup inside it" />
        </div>
        <div>
          <p>Backend Developing</p>
          <p>
            <b>Languages</b>
          </p>
          <p>Java, Kotlin, Node JS</p>
          <p>
            <b> Frameworks </b>
          </p>
          <div>
            <p>Spring Web</p>
            <p>Nest JS</p>
            <p>Express JS</p>
          </div>
          <p>
            <b>Development Tools</b>
          </p>
          <div>
            <p>Visual Studio Code</p>
            <p>Visual Studio</p>
            <p>Intelij IDEA</p>
            <p>Github</p>
            <p>Git</p>
          </div>
        </div>
      </div>
      <div class="skill3">
        <div>
          <img src="../assets/android.png" width="50px" alt="Android Icon" />
        </div>
        <div>
          <p>Android Developing</p>
          <p>
            <b>Languages</b>
          </p>
          <p>Java, Kotlin</p>
          <p>
            <b> Frameworks </b>
          </p>
          <div>
            <p>Jetpack Compose</p>
          </div>
          <p>
            <b>Development Tools</b>
          </p>
          <div>
            <p>Android Studio</p>
            <p>Github</p>
            <p>Git</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
section {
  min-height: 100vh;
  margin: 1em;
}

.greeting {
  background-color: crimson;
  transform: translateY(-5px);
  border-radius: 10px;

  padding: 1em;
  padding-bottom: 10em;
}

.greeting > :nth-child(1) {
  color: white;
  font-family: var(--secular);
  text-align: center;
  font-size: 30px;
}

.desc {
  color: white;
  font-family: var(--rubik);
  text-align: center;
  display: flex;
  justify-content: center;
}

.skillGrid {
  display: grid;
  grid-template-areas: "s1" "s2" "s3";
  grid-auto-columns: 1fr;
  background-color: #36413e;
  color: white;

  border-radius: 10px;
  transform: translateY(-100px);
  border: 5px solid crimson;
  margin-inline: 20px;
  overflow: hidden;

  box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
  -webkit-box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
  -moz-box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
}

.skillGrid > :nth-child(1) {
  grid-area: s1;
}

.skillGrid > * {
  padding-block: 20px;
  padding-inline: 20px;
}

.skillGrid > :nth-child(2) {
  border-block: 1px solid crimson;
}
.skillGrid > * > :nth-child(1) {
  text-align: center;
}

.skillGrid > * > :nth-child(2) {
  text-align: center;
}

.skillGrid > * > :nth-child(2) > :nth-child(1) {
  font-family: var(--secular);
  font-size: 20px;
}

.skillGrid > * > :nth-child(2) > * {
  font-family: var(--rubik);
  font-size: 16px;
}

.skillGrid > * > :nth-child(2) > :nth-child(3) {
  font-size: 14px;
}

.skillGrid > * > :nth-child(2) > :nth-child(5) {
  font-size: 14px;
}

.skillGrid > * > :nth-child(2) > :nth-child(7) {
  font-size: 14px;
}

.skillGrid > :nth-child(2) {
  grid-area: s2;
}
.skillGrid > :nth-child(3) {
  grid-area: s3;
}

.desc > p {
  max-width: 70ch;
}

@media (min-width: 992px) {
  .skillGrid {
    grid-template-areas: "s1 s1 s2 s2 s3 s3";
  }

  .skillGrid > :nth-child(2) {
    border-block: transparent;
    border-inline: 1px solid crimson;
  }
}

@media (min-width: 1200px) {
  .skillGrid {
    margin-inline: 100px;
  }
}
</style>
