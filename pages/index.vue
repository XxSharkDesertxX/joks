<template>
    <div :id="dark">
        <h1> THE  JOKE SITE ...</h1> 
        <h3>Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum?</h3>

       <v-btn @click="changemode">
          <v-icon>
          mdi-{{theme ? on : off}}
          </v-icon>
       </v-btn>
       
    </div>
</template>

<script>
export default {
  name: 'IndexPage',

  data() {
    return {
        dark:"main_home",
        theme:true,
        on: "lightbulb-on",
        off: "lightbulb-off"
    }
  },

  head(){
    return{
      title:"Home Page"
    }
  },

  methods: {
    changemode(){
        if (this.theme) {
          this.dark = "main_home_dark"
          this.theme = false;
        }else{
          this.dark = "main_home"
          this.theme = true;
        }
    }
  },


}
</script>

<style lang="css">
  #main_home{
    height: 80vh;
    display: flex; justify-content: center; align-items: center;
    flex-direction: column;
    user-select: none;
  }

  #main_home_dark{
    background: gray;
    color: #fff;
        height: 80vh;
    display: flex; justify-content: center; align-items: center;
    flex-direction: column;
    user-select: none;
  }

  #main_home h3{
      color: gray;
  }
</style>