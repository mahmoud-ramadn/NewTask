<template>
  <div class=" w-full ">
    <div class="  h-12    bg-primary">
    </div>
<!-- banner  -->

<div class=" container mx-auto  mt-14">

   <div class=" md:w-[1170px] mx-auto      grid md:grid-cols-6   grid-cols-1  gap-8 justify-center h-full ">

    <div class="   md:col-span-2  col-span-1  flex  flex-col justify-between gap-8 ">

      <div class=" w-full flex  flex-col       gap-7  h-[371px] rounded-sm  px-5   py-4 bg-[#E5E5E5]">
        <h4 class="  text-darkblue font-semibold text-lg ">ACCESORIES</h4>

         <div  class=" w-full space-y-[20px] h-[269px]  overflow-y-scroll   ">

           <div v-for="(item,index) in AccesoriseBtn" :key="index">
             <button class=" w-full flex justify-between group hover:text-blue items-center  text-darkblue font-semibold "> {{ item.titel }} <span class=" text-secondary group-hover:text-blue ">{{ item.num }}</span></button>


           </div>


         </div>

      </div>

      <div class=" w-full  h-[141px] text-darkblue  flex flex-col justify-between font-semibold bg-[#E5E5E5] p-5 ">
       <h3 class="  text-lg">PRICES</h3>
       <div>
       <p class=" w-full flex  text-sm justify-between items-center">Ranger:  <span class="   font-thin">${{value }}</span></p>
        <div class="slider-demo-block">
    <el-slider v-model="value" range show-stops :max="10" />
  </div>
       </div>

      </div>

      <div class=" w-full  h-[123px]  text-darkblue  flex flex-col justify-between font-semibold p-5  bg-[#E5E5E5]">
        <h3 class="  text-lg">COLOR</h3>



      </div>

      <div class=" w-full flex  flex-col       gap-7  h-[245px] rounded-sm  px-5   py-4 bg-[#E5E5E5]">
        <h4 class="  text-darkblue font-semibold text-lg ">BRAND</h4>

         <div  class=" w-full space-y-[20px] h-[269px]  overflow-y-scroll   ">

           <div v-for="(item,index) in AccesoriseBtn" :key="index">
             <button class=" w-full flex justify-between group hover:text-blue items-center  text-darkblue font-semibold "> {{ item.titel }} <span class=" text-secondary group-hover:text-blue ">{{ item.num }}</span></button>


           </div>


         </div>

      </div>

      <button class="  h-14 text-darkblue bg-[#E5E5E5] rounded ">
        MORE
      </button>






    </div>

    <div class="  h-full   md:col-span-4 col-span-1 bg-green-400">
s
    </div>


   </div>


</div>






  </div>
</template>

<script setup lang="ts">
const value = ref([13.99 ,25.99]);



 const AccesoriseBtn=[
   {
      titel:'Apple Car',
      num:'12'
   },
   {
      titel:'Air port & wireless',
      num:'12'
   },
   {
      titel:'Cables & Docks',
      num:'12'
   },
   {
      titel:'Cases & Films',
      num:'12'
   },
   {
      titel:'Charging Devices',
      num:'12'
   },
   {
      titel:'Connected home',
      num:'12'
   },
   {
      titel:'Headphones',
      num:'12'
   },
 ]

const selectedCity = ref("");

// Function to handle city selection
const selectCity = (cityName:string) => {
  selectedCity.value = cityName;
};
</script>
