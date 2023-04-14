<script>
import DcComics from "../data/dc-comics.json";
import CardComic from "./CardComic.vue";
export default {
    name: 'SiteMain',
    components: {
        CardComic
    },
    data() {
        return {
            comics: DcComics
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
        <section class="jumbo">
            <img src="../assets/img/jumbotron.jpg" alt="">
        </section>
        <section class="showcard ">
            <div class="container position-relative">
                <div class="current_series p-2 text-center position-absolute">
                    <h3>CURRENT SERIES</h3>
                </div>
                <div class="row row-cols-6 py-5">
                    <CardComic v-for="comic in comics" :src="comic.thumb" :title="comic.series"></CardComic>
                </div>
                <a name="" id="" class="btn load_more position-absolute rounded-0" href="#" role="button">
                    <span class="text-white"><strong>Load More</strong></span>
                </a>
            </div>
        </section>
    </main>
</template>