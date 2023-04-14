<script>
import JumboScreen from './JumboScreen.vue'
import ShowCard from "./ShowCard.vue";
export default {
    name: 'SiteMain',
    components: {
        ShowCard,
        JumboScreen
    },
    data() {
        return {
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
    <main>
       <JumboScreen></JumboScreen>
        <ShowCard></ShowCard>
    </main>
</template>