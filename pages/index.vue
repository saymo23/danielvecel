<template>
<div class="relative">
  <div id="card">
    <div id="backCard" class="transform -skew-y-6 rotate-6 sm:rounded-3xl"></div>
    <div id="datos">
      <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" focusable="false" width="2rem" height="2rem" style="-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);" id='menu' preserveAspectRatio="xMidYMid meet" viewBox="0 0 20 20"><path d="M16.4 9H3.6c-.552 0-.6.447-.6 1c0 .553.048 1 .6 1h12.8c.552 0 .6-.447.6-1c0-.553-.048-1-.6-1zm0 4H3.6c-.552 0-.6.447-.6 1c0 .553.048 1 .6 1h12.8c.552 0 .6-.447.6-1c0-.553-.048-1-.6-1zM3.6 7h12.8c.552 0 .6-.447.6-1c0-.553-.048-1-.6-1H3.6c-.552 0-.6.447-.6 1c0 .553.048 1 .6 1z" fill="#626262"/></svg>
      <img src="../static/me.jpg" alt="Me" class="me w-64" />
      <h1 >
        <span class="font-bold text-gray-600">DANIEL</span> SANTARRIAGA
      </h1>
      <h2 >
        Fullstack Developer Web
      </h2>
      <p>
        Full Stack Web Developer.
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
#backCard{
  @apply absolute bg-gray-200   bg-gradient-to-r from-orange-400 to-red-400 rounded-lg z-0;
  width: 450px;
  height: 100%;
  transform: rotate(-6deg)
}

#card {
  @apply relative  ;
  width: 450px;
  #datos{
    @apply flex flex-col justify-center items-center z-10 relative flex justify-center items-center text-center  bg-gray-200 h-auto p-12 rounded-lg shadow-lg z-20;
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
    #menu{
      @apply absolute z-30 cursor-pointer;
      left: 1rem;
      top: 1rem;
      &:hover > path{
        fill: #975a16
      }
    }
  }
  
}

</style>