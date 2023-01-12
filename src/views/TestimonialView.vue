<template>
    <div>
        <TestimonialVue />
        <RouterView />
    </div>
</template>

<script>
import TestimonialVue from '../components/Testimonial.vue';

export default{
    name: 'TestimonialView',
    components: {
    TestimonialVue
    }
}
</script>

<style scoped>
</style>