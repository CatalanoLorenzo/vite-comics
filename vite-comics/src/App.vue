<script >
import SiteHeader from "./components/SiteHeader.vue";
import SiteMain from "./components/SiteMain.vue"
import SiteFooter from "./components/SiteFooter.vue"
export default {
  components : {
    SiteHeader,
    SiteMain,
    SiteFooter
  },
  data() {
    return {

    }
  }
}
</script>

<template>

  <SiteHeader></SiteHeader>
  <SiteMain></SiteMain>
  <SiteFooter></SiteFooter>
  
</template>