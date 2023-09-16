<script setup>
const itens = defineProps(['item'])

</script>

<template>
    <div>
    <div class="card">
        <a
        :href="itens.item.href"
        >
            <img :src="itens.item.img" alt="Icone do servico" />
        </a> 
    </div>
     
    <div class="titulo" >
        <span>{{ itens.item.titulo }}</span> 
    </div>
   </div>
  
</template>


<style scoped>

img{
    width: 80px;
}

img:hover{
    zoom: 150%
    
    
}
span{
    font-weight: 600;
    font-size: large;
}
.card{
    margin: 20px 50px 20px 50px;
    display: block;
    width: 100px;
    
    background-color: rgb(255, 255, 255);
    display: flex ;
    justify-content: center;
    flex-direction: column;
    min-width: 125px;
    min-height: 125px;
    border: 1px solid rgb(25, 185, 46);
    border-radius: 120%;
    opacity: .9;
    box-shadow: 0 0 2em rgb(160, 228, 197);
    transition: box-shadow .5s;
}
.card:hover{
    opacity: 10;
    box-shadow: 0 0 4em rgba(65, 145, 177, 0.884);
    
    
}
.titulo{
    margin-top: 5%;
    color: rgb(255, 255, 255);
    opacity: 1;
    justify-content:center;

}
@media ( max-width: 600px ) {
    div{
        margin: 20px 20px 20px 20px;
    }
}

</style>