<script>
import ShopMenu from "../data/shopMenu"
import About from "../data/about"
import IconSrc from "../data/iconsrc";
export default {
    name: 'SiteFooter',
    data() {
        return {
            shopMenu:ShopMenu,
            about:About,
            iconsrc:IconSrc
        }
    },
}
</script>
<template>
    <footer>
        <section class="top text-white m-auto">
            <div class="container">
                <div class="row flex-column">
                    <div class="col">
                        <nav class="navbar navbar-expand-sm shop p-3">
                            <div class="container-fluid ">
                                <div class="py-3" v-for=" element in shopMenu">
                                    <a class="navbar-brand" :href="element.href">
                                        <img class="m-2" :src="element.src" alt="element.text">
                                        <span>{{element.text}}</span>
                                    </a>
                                </div>
                            </div>
                        </nav>
                    </div>
                </div>
            </div>
        </section>

        <section class="center p-3">
            <div class="container">
                <div class="row">
                    <div class="col">
                        <nav class="navbar navbar-expand-sm contacts">
                            <div class="container-fluid p-0">
                                <section class="py-1 d-flex flex-column h-100" v-for="element in about">
                                    <h4 class="text-white">{{element.title}}</h4>
                                    <ul class="px-0 list-unstyled">
                                        <li v-for="(,index) in element.link">
                                            <a class="text-decoration-none text-white" href="#" >{{element.link[index]}}</a>
                                        </li>
                                    </ul>
                                </section>
                            </div>
                        </nav>
                    </div>
                </div>
            </div>
        </section>

        <section class="bottom py-1">
            <div class="container py-2">
                <div class="row justify-content-between py-4">
                    <div class="col">
                        <a name="" id="" class="btn text-white border-1 border-primary" href="#" role="button">SIGN-UP
                            NOW!</a>
                    </div>
                    <div class="col d-flex justify-content-end">
                        <div class="followUs d-flex py-2 ">
                            <h4 class="text-white px-3 d-flex align-items-center">Follow US</h4>
                            <div class="icon">
                                <img class="m-1" :src="element.src" alt="" v-for="element in iconsrc">
                            </div>
                        </div>
                    </div>
                </div>
            </div>

        </section>

    </footer>
</template>