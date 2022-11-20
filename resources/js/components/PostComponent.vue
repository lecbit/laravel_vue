<template>
    <div>
        Vue 123213123
        <SinglePostComponent></SinglePostComponent>
        <div>Name: {{ name }}</div>
        <div>{{ vasyaJob }}</div>
        <button @click="sayHello()">Hello</button>
        <button @click="sayHi()">Hi</button>
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
    },
    methods: {
        sayHello() {
            console.log('Hello');
        },
        sayHi() {
            console.log('Hi');
        }
    },
    computed: {
        vasyaJob() {
            return this.name + ' работает в булошной'
        }
    }
}
</script>