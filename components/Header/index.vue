<template  >

  <div>
   
     <div class=" h-10  border-b ">
       <div class="md:container w-full  px-2  mx-auto h-full flex items-center justify-between ">
   
      <div class=" space-x-2  text-sm  text-darkblue " >
       <span>En <Icon name="iconamoon:arrow-down-2-fill" width="36px" height="36px" /></span>
       <span>USD <Icon name="iconamoon:arrow-down-2-fill" width="36px" height="36px" /></span>
      </div>
   
   
      <div class=" space-x-3  text-sm  flex items-center text-darkblue " >
       <span> <Icon name="uil:user" width="36px" height="36px" /> My profile</span>
       <p class=" flex items-center gap-x-1"><Icon name="icons8:box" width="16px" height="16px" />0Items <span class="  text-primary">$0.00</span> </p>
   
       <Icon class="  text-primary " name="lucide:search" width="15px" height="15px" />
      </div>
   
   
   
       </div>
     </div>
   
   
     <div class=" md:w-[640px] w-full mx-auto flex my-10  flex-col  justify-between items-center  h-[90px]">
        <img src="../../public/img/logo.svg" alt="">
        <ul class=" w-full   flex items-center justify-between  text-sm px-4">
          <li> <NuxtLink to="/"  active-class=" text-blue">Home</NuxtLink></li>
          <li> <NuxtLink to="/">Store</NuxtLink></li>
          <li> <NuxtLink to="/">IPHONE</NuxtLink></li>
          <li> <NuxtLink to="/">IPAD</NuxtLink></li>
          <li> <NuxtLink to="/">MACBOOK</NuxtLink></li>
          <li> <NuxtLink to="/">ACCESORIES</NuxtLink></li>
        </ul>
      </div>
 </div>

   
</template>

<script setup lang="ts">

</script>

<style scoped>

</style>
