<template>
      <div > 
          <Navbar/>
        <div>
              <Nuxt/>
        </div>
        <Footer/>
      </div>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {

    }
  }
}
</script>

<style lang="css">
    *{
      margin: 0; padding: 0;
      font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    }
</style>
