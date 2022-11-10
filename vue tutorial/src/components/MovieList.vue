<template >
   <ul class="movie-list list-group">
    <MovieListItem v-for="movie in movies" :key="movie" :movie="movie"/>
   </ul>
</template>
<script>
import MovieListItem from './MovieListItem.vue'
export default {
  components: { MovieListItem },
    props : {
      movies: {
      type: Array,
      required: true
     }
    }
}
</script>
<style scoped>
.movie-list{
  margin-top: 2rem;
  padding: 1rem;
  background-color: #fcfaf5;
  border-radius: 4px;
  box-shadow: 15px 15px 15px rgba(0,0,0,.15);
}    
</style>