<template>
  <div id="app">
  <button
      type="button"
      class="btn"
      @click="showModal"
    >
      ROLLBACK!
    </button>

    <modal
      v-show="isModalVisible"
      @close="closeModal"
    />

    <Navigation></Navigation>
    <router-view/>
  </div>
</template>

<script>
import Navigation from './components/Navigation'
import modal from './components/SecondModal.vue'
export default {
  name: 'App',
  components: {
    'Navigation': Navigation,
    'modal': modal
  },
  data () {
    return {
      isModalVisible: false
    }
  },
  methods: {
    showModal () {
      this.isModalVisible = true
    },
    closeModal () {
      this.isModalVisible = false
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
