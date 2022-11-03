<template>
  <div class="app">
    <div class="content">
      <Appinfo/>
      <div class="search-panel">
        <SearchPanel/>
      </div>
    </div>
  </div>
</template>
<script>
import Appinfo from '../components/Appinfo.vue'
import SearchPanel from '../components/SearchPanel.vue'
export default {
  components: { Appinfo, SearchPanel },
 
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