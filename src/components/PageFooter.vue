<script setup>
// Définition des props du composant
defineProps({
    site: {
        type: String,
        required: true
    }
})
</script>

<template>
    <footer>
        &copy; 2023 -
        <a :href="site">
            Supercell.com
        </a>
    </footer>
</template>

<style scoped lang="sass">
/*** Footer ***/
footer
    position: fixed
    z-index: 999
    bottom: 0
    height: 60px
    width: 100%
    background-color: black
    text-align: center
    padding: 1rem
    margin: 0

footer a
    color: white
</style>
