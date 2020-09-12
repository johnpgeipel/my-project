<template>
    <b-navbar toggleable="lg" type="dark" variant="danger" fixed="top">
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
        color: white;
    }

    .navCollapse {
        margin-left: 0rem;
    }

    @media screen and (min-width: 990px) {
        .navCollapse {
        margin-left: 2rem;
        }
    }

    .show {
        min-height: 100vh;
        text-align: center;
    }

    /* .show .navbarNav {
        margin: 0 auto;
    } */

    
</style>