<template>
<div>
  <div id="card">
    <div id="datos">
      <img src="../static/me.jpg" alt="Me" class="me w-64" />
      <h1 >
        <span class="font-bold text-gray-600">DANIEL</span> SANTARRIAGA  
        
      </h1>
      <h2 >
        Fullstack Developer Web
      </h2>
      <p>
        Soy desarrollador web por mi amor a crear cosas nuevas.
      </p>
      <Contacts />
    </div>
    
  </div>
</div>
</template>

<script>
export default {}
</script>

<style lang='scss'>
#card {
  @apply flex justify-center items-center text-center  bg-gray-200 h-auto p-12 rounded-lg shadow-lg ;
  width: 450px;
  #datos{
    @apply flex flex-col justify-center items-center;
    h1{
      @apply text-3xl font-thin  ;
    }
    h2{
      @apply text-xl text-orange-600 font-bold pb-2
    }
    p{
      @apply text-gray-600 mb-4;
    }
    .me{
      @apply rounded-full mb-4;
    }
    
  }
  
}

</style>