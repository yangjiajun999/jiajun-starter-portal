<template>
    <div>
        <treeset></treeset>
        <h1 v-for="(user) in users" :key="user.id">姓名：{{user.name}} 年龄：{{user.age}}</h1>
    </div>
</template>

<script>
import treeset from '../../components/TreeSet';

export default {
    name: 'homepage',
    layout: 'admin',
    components: {
        treeset
    },
    data() {
        return {
            users: [
                {
                    id: 1,
                    name: 'jack',
                    age: 10
                },
                {
                    id: 2,
                    name: 'tom',
                    age: 20
                }, {
                    id: 3,
                    name: 'cat',
                    age: 5
                },
            ]
        };
    }
};
</script>

<style scoped>

</style>
