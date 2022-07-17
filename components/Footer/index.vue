<template>
    <div id="footer">
        <v-btn class="icon_footer">
                <nuxt-link to="/" class="link_footer">
                    <v-icon  color="black" >
                        mdi-home
                    </v-icon>
                </nuxt-link>
        </v-btn>
    </div>
</template>

<script>
export default {

    methods: {
        backhome(){
            console.log(this.$route.fullPath);
        }
    },

}
</script>

<style scoped>
   #footer{
        height: 10vh;
        position: absolute;
        position: relative;
    }
    .icon_footer{
        position: absolute;
        right: 1rem; bottom: 1rem;
    }
    .link_footer{
        text-decoration: none;
        color: #000;
    }
</style>