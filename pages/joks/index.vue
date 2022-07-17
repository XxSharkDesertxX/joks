<template>
    <div >

        <Joks v-for="jok in joks" :key="jok.id"
            :id="jok.id"
            :jok="jok.joke"
        />

    </div>
</template>

<script>
import axios from 'axios'
export default {
 head(){
     return{
         title:"Joks page",
         meta:[
                {
                 hid:"discriptdsion",
                    name:"other dissdripation",
                    content:"this is a content for joks page"
             }
            ],
        }
    },




// asyncdata in vuex
    async asyncData( ) {
        const conf ={
            headers:{
                Accept : 'application/json'
            }
        }
        try {
            let res = await axios.get("https://icanhazdadjoke.com/search",conf)
            return {joks : res.data.results}
        } catch (error) {
            console.log(error);
        }
    },


// Async cerated vue :

//    async created(){
//         const config ={
//             headers:{
//                 Accept : "application/json"
//             }
//         }
//         try {
//             let res = await axios.get("https://icanhazdadjoke.com/search", config);h
//             this.joks = res.data.results
//         } catch (error) {             console.log(error);
//         }
//     }


}
</script>


<style lang="css" scope>
    h3{
        margin: 2rem;
    }
</style>