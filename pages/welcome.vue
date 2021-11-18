<template>
    <div>
        <h1>{{ $t('welcome') }}</h1>
    <nuxt-link :to="localePath('index')">{{ $t('index') }}</nuxt-link>
    </div>
</template>