<script setup>
// Définition des props du composant
defineProps({
    titre: {
        type: String,
        required: true
    },
    description: {
        type: String,
        required: true
    },
    site: {
        type: String,
        required: true
    }
})
</script>

<template>
    <header>
        <h1>{{ titre }}</h1>
        <p class="description"> {{ description }}</p>
        <a :href="site">
            <button>Site officiel</button>
        </a>
    </header>
</template>
