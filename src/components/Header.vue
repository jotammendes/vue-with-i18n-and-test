<template>
  <div>
    <select v-model="language" @change="handleLanguage">
      <option v-for="(lang, index) in languages" :key="index" :value="lang.name" :selected="lang.name === language">{{ lang.title }}</option>
    </select>
  </div>
</template>

<script>
  export default {
    name: 'Header',
    data() {
      return {
        languages: [
          {name: 'en', title: 'English'},
          {name: 'es', title: 'Espanhol'},
          {name: 'pt-BR', title: 'Português Brasileiro'}
        ],
        language: localStorage.getItem('language') || 'en'
      }
    },
    methods: {
      handleLanguage(event) {
        localStorage.setItem('language', event.target.value);
        window.location.reload();
      }
    }
  }
</script>

