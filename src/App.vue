<script>
import Loader from './components/Loader.vue'
import Form from './components/Form.vue'

export default {
  components: {
    Loader,
    Form
  },
  data() {
    return {
      zip:'',
    }
  },
  computed: {
    isValidZIP() {
      return this.zip.length === 5 && typeof this.zip === 'number'
    }
  }
}
</script>

<template>
  <header>
    <a href="/" class="main_link"> ZIP code</a>
  </header>

  <main >
    <Loader v-if="!isValidZIP"></Loader>
    
    <Form  v-else></Form>
  </main>
</template>


