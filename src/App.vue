<template>
  <div id="app">
    <HelloWorld msg="Code with Vue.Js Framwork" />
    <HomeView />
    <hr>
    <h1 style="text-align:center">Click Event on button </h1>
    <MyButton />
    <hr>
    <h1 style="text-align:center">Two way Binding </h1>
    <TwoWayBindComponent />
    <hr>
    <IfElse />
    <hr>
    <LoopsTypes />
    <br><br>
  </div>

</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import HomeView from './components/Home.vue';
import MyButton from './components/MyButton.vue';
import TwoWayBindComponent from './components/TwoWayBind.vue';
import IfElse from './components/IfElse.vue';
import LoopsTypes from './components/LoopTypes.vue';

export default {
  //  name: 'App', <= this is the root id which goes to main.js and it will mount to html
  name: 'App',
  // write here the file of the (for register the components)
  components: {
    HelloWorld,
    HomeView,
    MyButton,
    TwoWayBindComponent,
    IfElse,
    LoopsTypes,

  }
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Buenard&family=Kavivanar&display=swap');

* {
  font-family: 'Buenard', serif;
}
</style>