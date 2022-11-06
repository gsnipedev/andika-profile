<script lang="ts">
export default {
  methods: {
    Mailme() {
      window.location.href = "mailto:andikawpb200@gmail.com";
    },
    Github() {
      window.location.href = "https://github.com/gsnipedev";
    },
    LinkedIn() {
      window.location.href = "https://www.linkedin.com/in/andika-wahyudi-4bb655240/";
    },
  },
};
</script>

<template>
  <section id="footer">
    <div>
      <p>Start a project</p>
    </div>
    <div>
      <p>Interested in working together? We should queue up a time to chat.</p>
    </div>
    <div>
      <button>Let's do this</button>
    </div>
  </section>
  <footer>
    <div class="image">
      <div class="person">
        <img src="andika.jpeg" alt="" width="80" />
      </div>
    </div>
    <div class="quote">
      <p>
        Living, learning, & programming <br />
        one day at a time
      </p>
    </div>
    <div class="buttonContainer">
      <button @click="LinkedIn">In</button>
      <button @click="Github">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="25"
          height="25"
          fill="currentColor"
          class="bi bi-github"
          viewBox="0 0 16 16"
        >
          <path
            d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"
          />
        </svg>
      </button>
      <button @click="Mailme">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="25"
          height="25"
          fill="currentColor"
          class="bi bi-envelope"
          viewBox="0 0 16 16"
        >
          <path
            d="M0 4a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v8a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V4Zm2-1a1 1 0 0 0-1 1v.217l7 4.2 7-4.2V4a1 1 0 0 0-1-1H2Zm13 2.383-4.708 2.825L15 11.105V5.383Zm-.034 6.876-5.64-3.471L8 9.583l-1.326-.795-5.64 3.47A1 1 0 0 0 2 13h12a1 1 0 0 0 .966-.741ZM1 11.105l4.708-2.897L1 5.383v5.722Z"
          />
        </svg>
      </button>
    </div>
    <div class="closing">
      <p>Handcrafted with &hearts; by me &#169; Andika Wahyudi</p>
    </div>
  </footer>
</template>

<style scoped>
.closing {
  text-align: center;
  font-family: var(--rubik);
  color: white;
  margin-top: 2em;
}
.quote {
  color: white;
  filter: brightness(0.9);
  font-family: var(--inter);
  text-align: center;
  font-size: 22px;
  margin-block: 3em;
}

.buttonContainer {
  display: flex;
  justify-content: center;
}

.buttonContainer > button {
  transition: 0.2s;
  border-radius: 9999px;
  width: 50px;
  aspect-ratio: 1;
  margin-inline: 10px;
  border: 2px solid white;
  color: white;
  font-family: var(--inter);
  font-weight: bold;
  font-size: 25px;
  background-color: var(--crimson);
  display: flex;
  align-items: center;
  justify-content: center;
}
.buttonContainer > button:hover {
  background-color: var(--dark);
  cursor: pointer;
}
.image {
  display: flex;
  justify-content: center;
}
.person {
  border-radius: 100%;
  overflow: hidden;
  width: 80px;
  aspect-ratio: 1;
  border: 3px solid white;
  box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
  -webkit-box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
  -moz-box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
}

section {
  background-color: var(--dark);
  margin-inline: 2em;

  border-radius: 10px;
  transform: translateY(50%);

  box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
  -webkit-box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
  -moz-box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
  grid-template-areas: "title" "desc" "btn";
  display: grid;

  grid-auto-columns: 1fr;
  padding-inline: 1em;
  padding-block: 2em;
}

section > * {
  text-align: center;
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
}

section > :nth-child(3) > button {
  transition: 0.2s;
  background-color: var(--dark);
  border: transparent;
  font-size: 18px;
  padding-block: 10px;
  padding-inline: 40px;
  color: white;
  font-family: var(--rubik);
  border: 3px solid crimson;
  border-radius: 9999px;
  outline: none;
}
section > :nth-child(3) > button:hover {
  cursor: pointer;
  background-color: crimson;
  box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
  -webkit-box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
  -moz-box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
}
section > :nth-child(1) {
  grid-area: title;
  font-family: var(--secular);
  font-size: 32px;
}

section > :nth-child(2) {
  grid-area: desc;
  font-family: var(--rubik);
}

section > :nth-child(3) {
  grid-area: btn;
}

footer {
  margin: 1em;
  margin-top: 0px;
  padding-top: 15em;
  background-color: crimson;
  min-height: 450px;
  border-radius: 10px;
}

@media (min-width: 992px) {
  footer {
    padding-top: 8em;
  }
  section {
    margin-inline: 5em;
    padding-block: 1em;
    grid-template-areas: "title title desc desc btn btn";
  }
}

@media (min-width: 1200px) {
  section {
    padding-block: 1em;
    margin-inline: 10em;
    grid-template-areas: "title title desc desc btn btn";
  }
}

@media (min-width: 768px) {
}
</style>
