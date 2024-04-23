<script>
import { RouterLink, RouterView } from 'vue-router' // eslint-disable-line
import themeSwitcher from './components/theme/themeSwitcher.vue'
import layoutContainer from './components/layout/layoutContainer.vue'
import navNavbar from './components/nav/navNavbar.vue'

export default {
  data() {
    return {}
  },
  components: { themeSwitcher, layoutContainer, navNavbar }
}
</script>

<template>
  <header>
    <navNavbar></navNavbar>
    <themeSwitcher></themeSwitcher>
    <layoutContainer>
      <!-- <div class="wrapper">
          <nav>
            <RouterLink to="/">Home</RouterLink>
            <RouterLink to="/about">About</RouterLink>
          </nav>
        </div> -->
    </layoutContainer>
  </header>

  <RouterView />
</template>

<style>
body {
  background-color: rgb(var(--background-color));
  color: rgb(var(--font-color));
  font-family: var(--font-family);
}

a {
  color: rgb(var(--link-color));
}

a:is(:hover, :focus, :active) {
  color: rgb(var(--font-color));
}

#navbar_title {
  font-size: 2em;
}
</style>
