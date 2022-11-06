<script lang="ts">
export default {
  data() {
    return {
      name: "Andika",
    };
  },
};
</script>

<template>
  <section id="profile">
    <div class="grid-container">
      <div class="AboutText">
        <b>Hello, i'm</b>
        <p>Andika Wahyudi Pratama Bintang</p>
        <span>Software Engineer (/sɒft.weər ˌenjə nir/)</span>
        <p>
          is a person who applies the principles of software engineering to design, develop, maintain, test, and
          evaluate computer software.
        </p>
        <button>Continue --></button>
      </div>
      <div class="imgContainer">
        <div class="imgBorder">
          <img src="andika.jpeg" alt="Picture of Andika Wahyudi" width="300" />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
section {
  min-height: 80vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

.GoldText {
  color: var(--gold);
}

button {
  width: 200px;
  padding-block: 10px;
  background-color: crimson;
  outline: none;
  border: transparent;
  color: white;
  font-size: 16px;
  border-radius: 5px;
  font-family: monospace;
}
button:hover {
  cursor: pointer;
  filter: brightness(0.9);
}

img {
  background-color: lime;
}

#imgContainer {
  display: flex;
  justify-content: center;
  width: 100%;
}

.AboutText {
  background-color: var(--black);
  padding: 1em;
  color: white;
  font-family: sans-serif;
  grid-area: txt;
}

.AboutText > :nth-child(2) {
  font-size: 22px;
}

.AboutText > :nth-child(3) {
  font-style: italic;
  padding-left: 10px;
  border-left: 4px solid crimson;
}

.AboutText > :nth-child(4) {
  padding-left: 10px;
  border-left: 4px solid crimson;
  max-width: 350px;
}

.AboutText :nth-child(1) {
  display: block;
  align-self: center;
  font-size: 30px;
}
.grid-container {
  border-radius: 10px;
  display: grid;
  margin: 1em;
  width: 100%;

  grid-template-areas: " img img img img img img" "txt txt txt txt txt txt";
}

.imgBorder {
  border-radius: 100%;
  overflow: hidden;
  border: 5px solid crimson;
  max-height: 300px;
  max-width: 300px;
  aspect-ratio: 1;
}

.imgContainer {
  width: 100%;
  display: flex;
  justify-content: center;
  grid-area: img;
}

@media (min-width: 992px) {
  .grid-container {
    width: 60%;
  }

  .grid-container > :nth-child(2) {
    order: 1;
  }
}

@media (min-width: 662px) {
  .grid-container {
    grid-template-areas: " txt txt txt  img img img";
  }
}
</style>
