<template>
 <div class="justify-content-between">
  <li class="List-group-item d-flex justify-content-between">
    <span class="List-group-item-label">{{movie.name}}</span>
    <input type="number" class="List-group-item-input" :value="movie.raqamlar">
  </li> 

  <div class="d-flex justify-content-center align-items-centar">
     <button type="button" class="btn-cookie btn-sm">
      <i class="fas fa-cookie"></i>
     </button>

     <button type="button" class="btn-trash btn-sm">
      <i class="fas fa-trash"></i>
     </button>

     <i class="fas fa-star"></i>

  </div>
 </div>  
</template>
<script>
export default {
  props:
    {
      movie:{
        type: Object,
        requared: true
      }
    }
  
}
</script>
<style scoped>
.list-group-item.like .fa-star{
  opacity: 1;
  transform: translate(0);
} 
</style>