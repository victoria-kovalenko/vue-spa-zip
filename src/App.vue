<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <header>
    <h1> ZIP code</h1>
  </header>

  <main>
    <div 
    class="input-group mb-3 input-group--all"
    >
      <div class="input-group--title">
        <h2 class="input-group--title_style"> Find the info by ZIP code</h2>
      </div>

      <div class="input-group--form">
        <input 
          type="text" 
          class="input-area" 
          placeholder="Please enter ZIP code" 
          aria-label="Please enter ZIP code" 
          aria-describedby="button-addon2">

        <button 
          class="btn btn-outline-secondary" 
          type="button" 
          id="button-addon2">
          Search
        </button>
      </div>
    </div>
  </main>
</template>

<style scoped>
.input-group--all {
  display: flex;
  flex-direction: column;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%);
  width: 400px;
  border: solid black 0.5px;
  border-radius: 20px;
}

.input-area {
  display: block;
}

.input-group--title {
  background-color: aquamarine;
  border-radius: 20px;
  /* p-bottom: 10px; */
}

.input-group--title_style {
  display: inline-block;
  border-radius: 20px;
}

.input-group--form {
  display: flex;
  justify-content: center;
}
/* header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
} */
</style>
