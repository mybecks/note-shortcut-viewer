<template>
  <div id="app">
    <header>HEader</header>
    <main>
      <Note :keyCode="keyCode"></Note>
      <Presets></Presets>
    </main>
    <footer>Footer</footer>
  </div>
</template>

<script>
import Note from './components/Note.vue';
import Presets from './components/Presets.vue';

export default {
  name: 'App',
  components: {
    Note,
    Presets,
  },
  data() {
    return {
      keyCode: '',
    };
  },
  mounted() {
    window.addEventListener('keydown', (e) => {
      this.keyCode = e.code;
    });
  },
};
</script>

<style>
html,
body {
  width: 100%;
  height: 100%;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  color: #2c3e50;
  /* margin-top: 60px; */
  min-height: 100%;
  display: flex;
  flex-direction: column;
  align-items: stretch;
}

main {
  flex-grow: 1;
  background-color: aliceblue;
  padding-bottom: 2.5rem;
  position: relative;
  vertical-align: middle;
}

header,
main,
footer {
  flex-shrink: 0;
  text-align: center;
}

footer {
  height: 2.5rem;
  padding: 0.5rem;
  vertical-align: middle;
}

header {
  padding: 1rem;
}

@import '~bootstrap/dist/css/bootstrap.css';
</style>
