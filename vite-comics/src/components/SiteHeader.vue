<script>
import logo from "../components/Logo.vue"
import NavHeader from './NavHeader.vue'
export default {
    name: 'SiteHeader',
    components:{
        logo,
        NavHeader,
    },
    data() {
        return {
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
                    <NavHeader></NavHeader>
                </div>
            </div>
        </div>
    </header>
</template>