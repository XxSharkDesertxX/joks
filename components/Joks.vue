<template>
    <div>

        <p>{{jok}}</p>

    </div>
</template>

<script>
export default {
    name:"Joks",
    props:[
        "jok",
        "id"
    ]

}
</script>

<style lang="css" scope>
    p{
        margin: 2rem;
    }
</style>