<template>
      <div> 
          <nuxt-link to="/">Home</nuxt-link>
          <nuxt-link to="/about">About</nuxt-link>
          <nuxt-link to="/joks">Joks</nuxt-link>

          <div>
              <Nuxt/>
          </div>
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
