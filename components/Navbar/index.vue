<template>
      <div id="container_navbar"> 
          <nuxt-link to="/" exact class="main_router">Home</nuxt-link>
          <nuxt-link to="/joks" class="main_router">Joks</nuxt-link>
          <nuxt-link to="/about" class="main_router">About</nuxt-link>
      </div>
</template>

<script>
export default {
  name: 'Navbar',
  data () {
    return {

    }
  }
}
</script>

<style scoped>
    #container_navbar{
        height: 10vh;
        background-color: lightseagreen;
        display: flex; justify-content: center;
        align-items: center;
    }
    .main_router{
        margin: 0 1rem;
        font-size: 1.3rem;
        font-weight: bolder;
        text-decoration: none;
        color: #000;
        border-bottom: 2px solid transparent;
    }
  
    .nuxt-link-active{
        color: #fff;
        border-bottom: 2px solid #fff;
        transition: all .3s ease;
        filter: drop-shadow(-2px 4px 1px #000);
    }

</style>