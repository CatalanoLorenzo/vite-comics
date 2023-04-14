<script >
export default {
    name: 'Logo',
    data() {
        return {
            src: '/src/assets/img/dc-logo.png',
            title: 'logo DC'
        }
    },
}
</script>

<template>
    <div class="logo p-2">
        <img :src="this.src" alt="this.title">
    </div>
</template>