<template>
  <div class="main">
        <Header :header="header"/>
        <div class="container">
        </div>    
  <section class="container">
    <div>
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
  </div> 
</template>

<script>
import Header from '~/components/Header.vue';

export default {
  components: {
    Header
  },
  data() {
    return {
      header: {
                title: "john's portfolio",
                subtitle: "hi, i'm a front-end web dev",
                text: "johnpgeipel@gmail.com"
      },
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
  /* min-height: 100vh; */
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
  /* color: #35495e; */
  letter-spacing: 1px;
}

.subtitle {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
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

