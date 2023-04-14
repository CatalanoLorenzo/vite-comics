<script>
import SignupButton from './SignupButton.vue';
import FollowUs from "./FollowUs.vue";
export default {
    name: 'FooterBottom',
    components: {
        FollowUs,
        SignupButton,
    }
}
</script>
<template>
    <section class="bottom py-1 position-relative">
        <div class="container py-2">
            <div class="row justify-content-between py-4">
                <div class="col">
                    <SignupButton></SignupButton>
                </div>
                <div class="col d-flex justify-content-end">
                    <FollowUs></FollowUs>
                </div>
            </div>
        </div>
    </section>
</template>