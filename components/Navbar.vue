<template>
    <b-navbar toggleable="lg" type="light" variant="light" fixed="top">
        <b-navbar-brand>
            <nuxt-link class="navbarBrand" to="/">JPG</nuxt-link>
        </b-navbar-brand>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" class="navCollapse" is-nav>
            <b-navbar-nav class="navbarNav">
                <b-nav-item>
                    <nuxt-link class="navbarLink" to="/about">About</nuxt-link>
                </b-nav-item>
                <b-nav-item>
                    <nuxt-link class="navbarLink" to="/works">Works</nuxt-link>
                </b-nav-item>
                <b-nav-item>
                    <nuxt-link class="navbarLink" to="/contact">Contact</nuxt-link>
                </b-nav-item>
            </b-navbar-nav>
        </b-collapse>
    </b-navbar>
</template>
<script>
export default {
    
}
</script>
<style lang="css" scoped>

    .navbarBrand,
    .navbarLink {
        color: black;
    }

    
</style>