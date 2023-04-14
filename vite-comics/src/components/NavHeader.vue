<script>
import headerMenu from "../data/headerMenu.js"

export default {
    name:'NavHeader',
    data() {
        return {
            listheaderMenu:headerMenu,
        }
    },
}
</script>
<template>
    <nav class="navbar navbar-expand-sm navbar-light py-0">
        <div class="container-fluid">
            <a class="py-5 h-100 px-1 text-decoration-none text-black p-1" :href="element.title"
                v-for="element in listheaderMenu">{{ element.title }}</a>
        </div>
    </nav>
</template>