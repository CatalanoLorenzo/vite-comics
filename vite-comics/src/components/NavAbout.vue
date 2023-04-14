<script>
import About from "../data/about"
export default {
    name:'NavAbout',
    data() {
        return {
            about: About,
        }
    },
}
</script>
<template>
    <nav class=" contacts d-flex align-items-start">
                            <div class="col-2 p-0 d-flex flex-wrap">
                                <section class="py-1 d-flex flex-column h-100 justify-content-end">
                                    <h4 class="text-white">{{ about[0].title }}</h4>
                                    <ul class="px-0 list-unstyled">
                                        <li v-for="(element,index) in about[0].link">
                                            <a class="text-decoration-none text-white"  href="#">{{ element }}</a>
                                        </li>
                                    </ul>
                                </section>
                                <section class="py-1 d-flex flex-column h-100 justify-content-end">
                                    <h4 class="text-white">{{ about[1].title }}</h4>
                                    <ul class="px-0 list-unstyled">
                                        <li v-for="(element,index) in about[1].link">
                                            <a class="text-decoration-none text-white"  href="#">{{ element }}</a>
                                        </li>
                                    </ul>
                                </section>
                            </div>
                            <div class="col-2 p-0 d-flex ">
                                <section class="py-1 d-flex flex-column h-100 justify-content-end" v-for="(element,index) in about">
                                    <h4 class="text-white" v-show="index != 0 && index != 1">{{ element.title }}</h4>
                                    <ul class="px-0 list-unstyled" v-show="index != 0 && index != 1">
                                        <li v-for="(element) in element.link">
                                            <a class="text-decoration-none text-white"  href="#">{{ element }}</a>
                                        </li>
                                    </ul>
                                </section>
                                
                            </div>
                        </nav>
</template>