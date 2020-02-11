<template>
  <div id="app" style="transition:background-color 0.3s;"
    class="min-h-screen flex items-center justify-center bg-brand-primary"
    :class="theme"
  >
  <div>
    <button @click="toggleTheme()" class="p-3 bg-brand-text-primary text-brand-primary rounded">
      {{ theme }}
    </button>
    <h1 class="text-5xl font-bold text-brand-text-primary">Hello from Tailwind.</h1>
    <p class="text-brand-text-secondary">
      This is a demo how to set up a theme switcher using Tailwincss
    </p>
  </div>

  </div>
</template>

<script>
export default {
  name: 'app',
  data() {
    return {
      theme: 'theme-light'
    }
  },
  methods: {
    toggleTheme() {
      this.theme = this.theme === 'theme-light' ? 'theme-dark' : 'theme-light'
    }
  }
}
</script>


<style src="./assets/tailwind.css">

