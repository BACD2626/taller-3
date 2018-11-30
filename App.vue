<template>
  <div id="app" >
    
     <div  v-if="mostrar == true  ">
        <div class="login card-panel green white-text center">
            <h1>INICIA SECION</h1>
            <input type=“text” placeholder="usuario" v-model="user" /><br> <br>
          
            <input type=“text” placeholder="pass" v-model="pass" /><br> <br>
            

            <button type="primary" @click="mostrar = false"> login</button>
        </div>  
      
     
     </div>

      <div v-if="mostrar == false  " >
     <formulario/>
     <br><br>
     <button type="primary" @click="mostrar = true"> salir</button>
     
    </div>

  </div>
</template>

<script>


import formulario from './components/formulario.vue'
export default {
  name: 'app',
  components:{
     formulario
  },
  data () {
    
    
    return {
      
      mostrar: true,
      
      
    }
  }
}
</script>

<style>

</style>
