<script lang="ts">
export default {
    props: ['title']
}
</script>

<template>
    <div class="row m-7 h-auto card bg-base-300 rounded-box">
        <p class="w-full pl-7 pt-7 font-bold">{{ title }}</p>
        <div class="m-7 grid grid-flow-row-dense grid-cols-3">
            <slot />
        </div>
    </div>
</template>