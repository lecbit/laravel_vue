<template>
    <div>
        Vue 123213123
        <SinglePostComponent></SinglePostComponent>
        <div>Name: {{name}}</div>
    </div>
</template>

<script>
import SinglePostComponent from './SinglePostComponent.vue';
export default {
    name: "PostComponent",
    components: {
        SinglePostComponent
    },
    data() {
        return {
            name: 'Vasya'
        }
    }
}
</script>