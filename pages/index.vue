<template>
  <div>
    <nuxt-link :to="switchLocalePath('en')">English</nuxt-link>
    <nuxt-link :to="switchLocalePath('fr')">Français</nuxt-link>
    <nuxt-link :to="switchLocalePath('es')">Spenish</nuxt-link>

    <p>{{ $t('welcome') }}</p>
    <p>{{ $t('hello.hello') }}</p>


    <nuxt-link :to="localePath('welcome')">{{ $t('welcome') }}</nuxt-link>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  head () {
    return this.$nuxtI18nHead()
  }
})
</script>
