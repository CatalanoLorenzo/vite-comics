<script>
import FooterTop from "./FooterTop.vue";
import FooterCenter from './FooterCenter.vue'
import FooterBottom from './FooterBottom.vue'
export default {
    name: 'SiteFooter',
    components: {
        FooterBottom,
        FooterTop,
        FooterCenter,
    },


}
</script>
<template>
    <footer>
        <FooterTop></FooterTop>
        <FooterCenter></FooterCenter>
        <FooterBottom></FooterBottom>
    </footer>
</template>