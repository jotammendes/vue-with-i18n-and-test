<template>
  <p>{{ $t('hello') }}</p>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'HelloI18n'
})
</script>

<i18n>
{
  "en": {
    "hello": "Hello i18n in SFC!"
  },
  "es": {
    "hello": "Hola i18n en SFC!"
  },
  "pt-BR": {
    "hello": "Olá i18n em SFC!"
  }
}
</i18n>
