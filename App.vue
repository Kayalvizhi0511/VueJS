<template>
  <div>
    //Text Binding
  <div>hello {{name}}</div>
  <div v-text="name"></div>
  //HTML Binding
  <div v-html="channel"></div>
  <div v-html="hack"></div>
  //Atrributes Binding
  <h2 v-bind:id="HeaderId">Kayal</h2>
  <button v-bind:disabled="isDisabled">Bind</button>
  </div>
</template>

<script>
export default {
  name: "App",
  data(){
    return {
  //Text Binding
  name: "kayal",
  //HTML Binding
  channel:'<b>hello</b>',
  hack: `<a href="#" onclick=alert("haked")> Win a prize </a>`,
  //Atrributes Binding
  HeaderId: 'Kayal',       
  isDisabled: true,       
  };
},
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
