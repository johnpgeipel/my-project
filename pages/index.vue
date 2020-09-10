<template>
  <section class="container">
    <div>
      <AppLogo/>
      <h1 class="title">
        portfolio
      </h1>
      <h2 class="subtitle">
        Nuxt.js project
      </h2>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          rel="noopener"
          class="button--green">Documentation</a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          rel="noopener"
          class="button--grey">GitHub</a>
      </div>
      <div class="portfolioItems">
        <h2 v-for="item in list"
            :key="item">
          {{ item }}</h2>
      </div>
      <div class="resumeItems">
        <h2 v-for="item in jobs"
            :key="item.name">
          {{ item.title }} : {{ item.date }}</h2>
      </div>
    </div>
  </section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
    AppLogo
  },
  data() {
    return {
      list: {
          line1: "Here is an item.",
          line2: "Here is an item.",
          line3: "Here is an item."
      },
      jobs: [
        {
          title: "Artist",
          date: "January 1, 2020"
        },
        {
          title: "Web Dev",
          date: "September 29, 2020"
        }
      ]
      
    }
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>

