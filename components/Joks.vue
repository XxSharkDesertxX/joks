<template>
    <div>

        <nuxt-link :to="`/joks/${id}`" class="routers">
            <p>* {{jok}}</p>
        </nuxt-link>

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
        font-size: 1.1rem;
        font-weight: normal;
        transition: all .6s;
        padding: .5rem;
    }
    p:hover{
        background: rgb(221, 221, 221);
    }
    .routers{
        text-decoration: none;
        color: #000;
    }
</style>