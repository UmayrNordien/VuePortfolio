<template>
    <div>
        <ProjectsVue/>
        <RouterView/>
    </div>
</template>

<script>
import ProjectsVue from '../components/Projects.vue'

export default {
    name:
    'ProjectsView',
    components: {
        ProjectsVue
    }
}
</script>

<style scope>
</style>