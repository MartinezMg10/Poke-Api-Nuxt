<template lang>
    <div>
       <p>{{  nombre }}</p>
       <img v-if="mostrar" src="../static/pexels-photo-3165335.jpeg" class="h-[150px]" alt="">
       <button  @click="cambiar" class=" bg-sky-500">Cambiar nombre</button>
    </div>
</template>

<script>
export default {
    data: () => ({
    nombre:"Miguel",
    mostrar:true
  }),

  methods:{
    cambiar(){
        this.nombre == "Miguel"  ? this.nombre = "Martinez" : this.nombre = "Miguel"
        this.mostrar =!this.mostrar
        }
    }
}
</script>
<style lang="">
    
</style>