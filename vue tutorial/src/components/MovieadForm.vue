<template>
    <div class="movie-add-form">
       <h3>Yangi kino qo'shish</h3>
       <form class="d-flex" @submit.prevent>
            <input 
            type="text" 
            class="form-control new-movie-label" 
            placeholder="Qanday kino" 
            v-model="name">

            <input 
            type="text" 
            class="form-control new-movie-label" 
            placeholder="Necha marotaba ko'rilgan" 
            v-model="viewers">
            <button class="btn btn-outline-dark" type="submit" @click="addMovie">Qo'shish</button>
       </form>
    </div>
</template>
<script>
export default {
    data() {
      return {
        name: "",
        viewers: ""
      }
    },
    methods: {
      addMovie(){
        const newMovie = {
          name: this.name,
          viewers:this.viewers,
          favorite: false
        }
        console.log(newMovie);
      }
    },
}
</script>
<style scoped>
.movie-add-form{
  margin-top: 2rem;
  padding: 1rem;
  background-color: #fcfaf5;
  border-radius: 4px;
  box-shadow: 15px 15px 15px rgba(0,0,0,.15);
}  
button{
 margin-top: 1rem;
}
</style>