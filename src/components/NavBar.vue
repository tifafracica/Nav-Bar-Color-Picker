<template>
  <nav id="navbar" v-if="color" :style="'background:'+color">
    <a href="#" class="home">Home</a>
    <a href="#" class="productos">Productos</a>
    <a href="#" class="servicios">Servicios</a>
    <a href="#" class="contactos">Contactos</a>
    <swatches
      v-model="color"
      
      :colors="colors"

      row-length="6"
      shapes="circles"
      show-border
      popover-to="left"
      
    ></swatches>
  </nav>
  
</template>

<script>
import Swatches from 'vue-swatches'
export default {
  components: {
    Swatches
  },
  data () {
    return {
      color: '#F64272',
      colors: ['#F64272', '#F6648B', '#F493A7', '#F891A6', '#FFCCD5', '']
    }
  },
  
  
}
</script>


<style scoped>
@import url('https://fonts.googleapis.com/css?family=Didact+Gothic');

*{
		margin:0;
		padding:0;
	}

a, a:visited {
		outline:none;
		color:#389dc1;
	}

a:hover{
  text-decoration:none;
}

#navbar {
  display:inline-block;
  background-color:#f8e1ee;
  border-radius:2px;
  margin-bottom: 2rem;
  width: 100%;
  display: flex;
  justify-content: space-between;
}

#navbar a{
		display:inline-block;
		padding: 18px 30px;
		color:white;
    font-family: 'Didact Gothic', sans-serif; 
		font-weight:bold;
		font-size:16px;
		text-decoration:none;
		line-height:1;
		text-transform: uppercase;
		background-color:transparent;

		-webkit-transition:background-color 0.25s;
		-moz-transition:background-color 0.25s;
		transition:background-color 0.25s;
	}

  #navbar a:last-child{
		border-radius:0 2px 2px 0;
	}

.vue-swatches{
  padding: 5px 20px 0 20px;
  background: white;
}


</style>



  



