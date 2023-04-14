<script>
export default {
    name: 'CardComic',
    props:
    {
        src: String,
        title: String,
    }
    ,
}
</script>

<template>
    <div class="col p-2">
        <div class="cards">
            <div class="  p-0">
                <div class="cover">
                    <img :src="src" class="card-img-top " alt="">

                </div>
            </div>
            <div class="title p-1">
                <h6 class="card-title text-white">{{ title }}</h6>
            </div>
        </div>
    </div>
</template>
<style lang="scss">

</style>