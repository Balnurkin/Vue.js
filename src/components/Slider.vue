<script>
export default {
    props: [
        'id', 
        'title', 
        'text'
    ],
    data: () => {
        return{

        }
    },
    methods:{

    }
}
</script>

<template>
    <div>
        <h1>{{title}}</h1>
        <p>{{text}}</p>
    </div>
</template>

<style scoped>
</style>