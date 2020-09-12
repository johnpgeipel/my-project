<template>
    <b-jumbotron class="header" bg-variant="danger" text-variant="white" border-variant="danger">
        <div class="headerContent">
            <h1 class="headerTitle title">{{ header.title }}</h1>
            <h3 class="headerSubtitle">{{ header.subtitle }}</h3>
            <hr class="my-4">
            <p>{{ header.text }}</p>
        </div>
    </b-jumbotron>
</template>

<script>
export default {
    props: {
        header: {
            type: Object,
            default: null
        }
    }
}
</script>

<style lang="css">

    .header {
        min-height: 70vh;
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
        background-color: red;
    }

    .headerSubtitle, .headerTitle, p {
        font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
        color: white;

    }
    
</style>