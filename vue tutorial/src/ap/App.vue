<template>
  <div class="app font-monospace">
    <div class="content">
      <Appinfo/>
      <div class="search-panel">
        <SearchPanel/>
        <AppFilter/>
      </div>
       <MovieList/>
       <MovieadForm/>
    </div>
  </div>
</template>
<script>
import AppFilter from '../components/AppFilter.vue'
import Appinfo from '../components/Appinfo.vue'
import MovieadForm from '../components/MovieadForm.vue'
import MovieList from '../components/MovieList.vue'
import SearchPanel from '../components/SearchPanel.vue'
export default {
  components: { Appinfo, SearchPanel, AppFilter, MovieList, MovieadForm },
 
}
</script>
<style>
.app{
    height: 100vh;
    color: #000;
}
.content{
  width: 1000px;
  min-height: 700px;
  background: #fff;
  margin: 0 auto;
  padding: 5rem 0;
}
.search-panel{
  margin-top: 2rem;
  padding: 1rem;
  background-color: #fcfaf5;
  border-radius: 4px;
  box-shadow: 15px 15px 15px rgba(0,0,0,.15);
}
</style>