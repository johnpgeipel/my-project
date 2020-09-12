<template>
  <div class="main">
        <Header :header="header"/>
        <div class="container">
        </div>    
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
                title: "contact",
                subtitle: "feel free to reach out to me",
                text: "johnpgeipel@gmail.com"
      }
    }
  }
}
</script>
<style lang="css" scoped>

    h1 {
        color: black;
    }

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
</style>