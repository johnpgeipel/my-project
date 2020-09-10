<template>
    <b-navbar toggleable="lg" type="light" variant="light" fixed="top">
        <b-navbar-brand>
            <nuxt-link to="/">JPG</nuxt-link>
        </b-navbar-brand>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
            <b-navbar-nav >
                <b-nav-item>
                    <nuxt-link to="/about">About</nuxt-link>
                </b-nav-item>
                <b-nav-item>
                    <nuxt-link to="/works">Works</nuxt-link>
                </b-nav-item>
                <b-nav-item>
                    <nuxt-link to="/contact">Contact</nuxt-link>
                </b-nav-item>
            </b-navbar-nav>
        </b-collapse>
    </b-navbar>
</template>
<script>
export default {
    
}
</script>
<style lang="css">

    nuxt-link {
        color: black;
    }
    
</style>