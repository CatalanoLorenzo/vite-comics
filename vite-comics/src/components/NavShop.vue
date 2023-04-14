<script>
import ShopMenu from "../data/shopMenu"
export default {
    name: 'ShopMenu',
    data() {
        return {
            shopMenu: ShopMenu,
        }
    },
    methods: {
        getImageUrl(name) {
            return new URL(`../assets/img/${name}.png`, import.meta.url).href
        }
    },
}
</script>
<template>
    <nav class="navbar navbar-expand-sm shop p-3">
        <div class="container-fluid ">
            <div class="py-3" v-for=" element in shopMenu">
                <a class="navbar-brand" :href="element.href">
                    <img class="m-2" :src="getImageUrl(element.src)" alt="element.text">
                    <span class="text-white">{{ element.text }}</span>
                </a>
            </div>
        </div>
    </nav>
</template>