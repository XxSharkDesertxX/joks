<template>
    <div class="alon_jok">
        <h3 >
            {{jok}}
        </h3>

            <v-btn class="btn_simple">
                <nuxt-link to="/joks" class="icon_simple">
                    <v-icon>
                        mdi-arrow-left
                    </v-icon>
                </nuxt-link>
            </v-btn>


    </div>
</template>

<script>
import axios from 'axios'

export default {


    async asyncData({ params }){
        const conf={
            headers:{
                Accept:"application/json"
            }
        }
        try {
            let rest = await axios.get(`https://icanhazdadjoke.com/j/${params.id}` , conf);
            console.log(rest.data.joke);
            return {jok : rest.data.joke}
        } catch (error) {
            console.log(error);
        }
    },


}
</script>

<style scoped>
    .alon_jok{
        height: 80vh;
        display: flex; justify-content: center; align-items: center;
    }
    h3{
        font-size: 2rem;
        font-weight: normal;
        user-select: none;
    }
    .icon_simple{
        color: black;
        text-decoration: none;
    }
    .btn_simple{
        position: absolute;
        top: 5rem;
        right: 1rem;
    }
</style>