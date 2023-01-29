<template>
     <div class="title">     </div>
        <h4> {{ title }} </h4>
      <nav>
        <router-link  to="/">Home</router-link>
        <router-link  to="/products">Products</router-link>
        <router-link  to="/profile">Profile </router-link>  
      </nav>
</template>

 <script lang="ts">
 import { defineComponent} from 'vue'
    

 export default defineComponent({
   name: 'NavBar',
   props: {
        title: {
            type: String,
            required: true,
        
},
},
 });
 </script>


<style scoped>
nav {
    width: 100%;
    display: flex;
    justify-content: space-between;
    background-color: aliceblue;
    padding: 30px;
    align-items: center;
}
h4 {
    color: rgb(0, 0, 0);
}
nav a {
  font-weight: bold;
  color: #2c3e50;
}
</style>