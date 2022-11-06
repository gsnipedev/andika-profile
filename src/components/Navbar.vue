<script lang="ts">
export default {
  data() {
    return {
      shouldDrop: false,
    };
  },
};
</script>

<template>
  <section class="navbarLG">
    <a href="">
      <h2>Andika</h2>
    </a>
    <ul>
      <li><a href="#profile">Home</a></li>
      <li><a href="#skill">Skills</a></li>
      <li><a href="#footer">Contact</a></li>
    </ul>
  </section>

  <section class="navbarSM">
    <div class="dropdown" @mouseleave="shouldDrop = false">
      <div class="nav">
        <button class="dropbutton" @mouseover="shouldDrop = true">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="32"
            height="32"
            fill="currentColor"
            class="bi bi-list"
            viewBox="0 0 16 16"
          >
            <path
              fill-rule="evenodd"
              d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5zm0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5zm0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5z"
            />
          </svg>
        </button>
        <div class="brand">Andika</div>
      </div>

      <div class="dropdownitem" :style="{ display: shouldDrop ? 'block' : 'none' }">
        <ul>
          <li><a href="#profile">Home</a></li>
          <li><a href="#profile">Skills</a></li>
          <li><a href="#profile">Contact</a></li>
        </ul>
      </div>
    </div>
  </section>
</template>

<style scoped>
.nav {
  display: grid;
  grid-template-columns: 50px auto;
}

.dropbutton {
  background-color: crimson;
  color: white;
  border: 1px solid transparent;
  outline: none;
}
.dropdownitem > ul > li > a {
  color: white;
  text-decoration: none;
}

.dropdownitem > ul > li {
  padding-block: 7px;
  padding-inline: 1em;
  border-radius: 5px;
  cursor: pointer;
}

.dropdownitem > ul > li:hover {
  background-color: var(--dark);
}

.dropdownitem > ul {
  list-style: none;
  color: white;
  font-family: var(--rubik);
  padding-inline: 1em;
}

.brand {
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-family: var(--rubik);
  font-size: 21px;
  font-weight: bold;
  transform: translateX(-20px);
}
.navbarSM {
  margin: 1em;
  padding-inline: 1em;
  background-color: crimson;
  border-radius: 10px;
  padding-block: 15px;
}
.navbarLG > a {
  color: #ffffff;
  text-decoration: none;
  font-family: var(--secular);
}

.navbarLG > ul {
  list-style: none;
  display: inline-flex;
}

.navbarLG > ul > li {
  margin-left: 20px;
  color: white;
  font-weight: bold;
}
.navbarLG > ul > li > a {
  text-decoration: none;
  color: white;
}

.navbarLG > ul :hover {
  filter: brightness(0.9);
  cursor: pointer;
}

.navbarLG {
  display: none;
  padding-inline: 100px;
  background-color: crimson;
  color: #ffffff;
  justify-content: space-between;
  align-items: center;
  margin: 1em;
  border-radius: 10px;
  box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
  -webkit-box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
  -moz-box-shadow: 0px 3px 5px -2px rgba(0, 0, 0, 0.75);
  font-family: "Open Sans", sans-serif;
}

@media (min-width: 662px) {
  .navbarLG {
    display: flex;
  }

  .navbarSM {
    display: none;
  }
}
</style>
