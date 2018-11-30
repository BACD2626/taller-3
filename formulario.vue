<template>
  <div>
      <h1>FORMULARIO DE ENTREGA</h1>
      
    <input type=“text” placeholder="nombre" v-model="nombre" />
    
    <br>
    <br>
    
    <input type=“text” placeholder="apellido" v-model="apellido" />
   
    <br>
    <br>
     
    <input type=“text” placeholder="ciudad" v-model="ciudad" />
    <br>
    <br>
    
    <input type=“text” placeholder="sexo" v-model="sexo" />
    <br>
    <br>
     
   <input type=“text” placeholder="fecha de nacimiento" v-model="fecha" />
    <br>
    <br>
     
    <input type=“text” placeholder="direccion de entrega" v-model="direccion" />
    <br> <br>

    <button type="primary" @click="mostrar = true"> mostrar datos</button>
    <button type="primary" @click="mostrar = false"> ocultar datos</button>
    
    <div  v-if="mostrar == true  ">
         <h1>datos de cliente</h1>
         
         <h2>
         ---------------------------- <br>   
         nombre: {{nombre}} <br>
          ---------------------------- <br>
         apellido: {{apellido}}<br>
          ---------------------------- <br>
         ciudad: {{ciudad}}<br>
          ---------------------------- <br>
         sexo: {{sexo}}<br>
          ---------------------------- <br>
         fecha: {{fecha}}<br>
          ---------------------------- <br>
         direccion: {{direccion}}<br>
         ---------------------------- 
         </h2>
    </div>
   
  </div>
</template>

<script>
export default {
  name:'',
  data () {
    return {
        mostrar:false,
        nombre: null,
        apellido: null,
        ciudad: null,
        sexo: null,
        fecha: null,
        direccion: null,
    }
  },
  methods:{
      onclick:function(){
          console.log(this.nombre)

          console.log(this.apellido)
      }
  }
}
</script>

<style>

</style>
