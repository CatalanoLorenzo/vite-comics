<script>
import headerMenu from "../data/headerMenu.js"
import logo from "../components/Logo.vue"
export default {
    name: 'SiteHeader',
    components:{
        logo
    },
    data() {
        return {
            listheaderMenu:headerMenu,

        }
    },
    
}
</script>

<template>
    <header>
        <div class="container">
            <div class="row justify-content-between align-items-baseline">
                <div class="col">
                    <logo></logo>
                </div>
                <div class="col ">
                    <nav class="navbar navbar-expand-sm navbar-light py-0">
                        <div class="container-fluid">
                            <a class="py-5 h-100 px-1 text-decoration-none text-black p-1" :href="element.title" v-for="element in listheaderMenu">{{element.title}}</a>
                        </div>
                    </nav>
                </div>
            </div>
        </div>
    </header>
</template>