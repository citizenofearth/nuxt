<template>
  <section class="container">
    <div>
      <logo />
      <h1 class="title">
        About Page
      </h1>
      <nuxt />
    </div>
    <div>
      <p>
        <button @click="$store.commit('increment')">
          {{ $store.state.counter }}</button
        ><br />>
        <NuxtLink to="/">
          Home
        </NuxtLink>
      </p>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 50px;
  color: #35495e;
  letter-spacing: 1px;
}
</style>
