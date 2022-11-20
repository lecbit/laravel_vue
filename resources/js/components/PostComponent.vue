<template>
    <div>
        <table class="table">
            <thead>
                <tr>
                    <th scope="col">ID</th>
                    <th scope="col">Имя</th>
                    <th scope="col">Возраст</th>
                    <th scope="col">Должность</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="person in persons">
                    <th scope="row">{{person.id}}</th>
                    <td>{{ person.name }}</td>
                    <td>{{ person.age }}</td>
                    <td>{{ person.job }}</td>
                </tr>
            </tbody>
        </table>
    </div>
</template>

<script>
import SinglePostComponent from './SinglePostComponent.vue';
export default {
    name: "PostComponent",
    data() {
        return {
            persons: [
                {
                    id: 1,
                    name: 'Vasya',
                    age: 20,
                    job: 'coach'
                },
                {
                    id: 2,
                    name: 'Kolya',
                    age: 24,
                    job: 'developer'
                },
                {
                    id: 3,
                    name: 'Borya',
                    age: 23,
                    job: 'driver'
                },
            ]
        }
    },
}
</script>