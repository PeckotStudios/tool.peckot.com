<script lang="ts">
export default {
    props: ['tool', 'name', 'desc']
}
</script>

<template>
    <a :href="`/${tool}`" class="card card-side mx-2 my-2 bg-base-100 shadow-xl transition hover:scale-105">
        <figure class="m-2 w-16 h-auto"><img draggable="false" :src="`/assets/${tool}.png`" /></figure>
        <div class="card-body px-2 py-5">
            <h2 class="card-title text-sm">{{ name }}</h2>
            <p class="text-sm text-left">{{ desc }}</p>
        </div>
    </a>
</template>