<template>
    <div>
        <ResumeVue/>
        <RouterView/>
    </div>
</template>

<script>
import ResumeVue from '../components/Resume.vue'

export default {
    name: 'ResumeView',
    components: {
        ResumeVue
    }
}
</script>