<template>
  <main class="body">
    <!-- <div class="one">
      
    </div>
    <div class="two" name="two">
      two的内容显示
    </div> -->
    <AppTodos v-if="todos[0].content[0].isShow" />
    <AppTwo v-if="todos[1].content[0].isShow" />
  </main>
</template>

<script type="text/ecmascript-6">

  import AppTodos from "./ex1/AppTodos";
  import AppTwo from "./ex2/AppTwo";

  export default {
    components:{
      AppTodos,
      AppTwo,
    },
    props:['todos'],
    
  }
</script>

<style scoped>
/* main */
.body{
  margin: 200px 0px 0px;
  background-color: #efefef;
  height: 80vh;
}

</style>
