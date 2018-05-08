<template>
  <div id="app">
    <!--<img src="./assets/logo.png">
    <router-view/>
    <h1>{{msg}}</h1>-->
    <headers></headers>
    <tab></tab>
   
  </div>
</template>

<script>
	
	import headers from './components/headers.vue'
	import tab from './components/tab.vue'
export default {
     data(){
     	 return{
     	 	 msg:'vue 真垃圾'
     	 }
     },
      components: {headers,tab}
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

}
</style>
