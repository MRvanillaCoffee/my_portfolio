<script>
  export default{
    name: 'app',
    data(){
      return{
        firstName:'Thanakorn',
        lastName:'Sertsai',
        picture:'img/IMG_20260220_184928.jpg'
      }
    },

    methods:{
    getFullName(){
      return this.firstName + ' ' + this.lastName
    }
  }
  }

  
</script>

<template>
  <section>
    <nav class="navbar bg-dark">
      <div class="container-fluid">
            <a class="navbar-brand text-white" href="#"><h3>Thanakorn</h3></a>
            <div>
              <a class="navbar-brand text-white" href="#"><h3>Skill</h3></a>
              <a class="navbar-brand text-white" href="#"><h3>About</h3></a>
            </div>
            
      </div>
    </nav>
    <div class="container-fluid">

      <h2>This website is {{ getFullName()}}'s portfolio</h2>
      <img v-bind:src="picture" width="400">
    </div>
  </section>
</template>

<style>

</style>
