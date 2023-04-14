<script>
import NavShop from './NavShop.vue';
export default {
    name: 'FooterTop',
    components:{
        NavShop,
    }
}
</script>
<template>
    <section class="top text-white m-auto">
        <div class="container">
            <div class="row flex-column">
                <div class="col">
                    <NavShop></NavShop>
                </div>
            </div>
        </div>
    </section>
</template>