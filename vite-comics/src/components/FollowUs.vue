<script>
import IconSrc from "../data/iconsrc";
export default {
    name:'IconSrc',
    data() {
        return {
            iconsrc:IconSrc,
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
    <div class="followUs d-flex py-2 ">
        <h4 class="text-white px-3 d-flex align-items-center">Follow US</h4>
        <div class="icon">
            <img class="m-1" :src="getImageUrl(element.src)" alt="" v-for="element in iconsrc">
        </div>
    </div>
</template>