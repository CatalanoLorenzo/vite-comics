<script>
import NavAbout from "./NavAbout.vue";
export default {
    name:'FooterCenter',
    components:{
        NavAbout,
    }
}
</script>
<template>
    <section class="center p-3 position-relative">
        <div class="container ">
            <div class="row">
                <div class="col">
                    <NavAbout></NavAbout>
                </div>
            </div>
        </div>
    </section>
</template>