<template>
    <div class="app-info">
        <p class="fs-3 text-upercase">Barcha kinolar soni: {{kinoSoni}}</p>
        <p class="fs-4 text-upercase">Ko'rilgan kinolar soni:{{korilganlarSoni}}</p>
    </div>
</template>
<script>
export default {
    props:{
        kinoSoni:{
            type: Number,
            requared: true
        },
        korilganlarSoni:{
            type: Number,
            requared: true
        }
    }
}
</script>
<style scoped>
.app-info{
 padding: 1.5rem;
 background-color: #fcfaf5;
 border-radius: 4px;
 box-shadow: 15px 15px 15px rgba(0,0,0,.15);
}  
</style>