<template>
  <div class="about">
    <h1>{{ $t('aboutPage') }}</h1>
    <HelloI18n />
  </div>
</template>

<script>
  import HelloI18n from '@/components/HelloI18n.vue';

  export default {
    name: 'About',
    components: {
      HelloI18n
    }
  }
</script>
