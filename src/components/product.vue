<script setup>

import Card from "./card.vue";
import {ref} from "vue";

const product = ref([
  {
    title:"",
    image:'src/assets/Elements-20230930T071855Z-001/Elements/Frame 36.png'
  },  {
    title:"",
    image:'src/assets/Elements-20230930T071855Z-001/Elements/Frame 51.png'
  },  {
    title:"",
    image:'src/assets/Elements-20230930T071855Z-001/Elements/Frame 52.png'
  },  {
    title:"",
    image:'src/assets/Elements-20230930T071855Z-001/Elements/Frame 53.png'
  },  {
    title:"",
    image:'src/assets/Elements-20230930T071855Z-001/Elements/Frame 54.png'
  },  {
    title:"",
    image:'src/assets/Elements-20230930T071855Z-001/Elements/Frame 55.png'
  },
])

</script>

<template>


<div class="grid grid-cols-2  justify-items-center justify-center gap-4  pl-40 pr-40 mt-10 " >
  <div class="w-full flex flex-col justify-center items-center"  v-for="item in product">
    <div class="w-full rounded  hover:border-blue-950 hover:border-4" >
      <div class=" relative overflow-hidden group  bg-cover bg-center"  style="background-image: url('src/assets/Background-20230930T071856Z-001/Background/Frame 39.png');" >
        <div class="flex flex-row justify-center h-[550px] ">
          <div class="justify-items-end mt-24">
            <img
                :src="item.image"
                alt="Card Image"
                class="w-44 h-auto transition-transform transform hover:scale-125  "
            />
          </div>
          <div>

          </div>
        </div>
        <div class="card-details absolute inset-0 flex flex-col justify-end opacity-0 group-hover:opacity-100 transition">
          <div class="text-white text-center ">
            <div class="bg-blue-500 text-white px-4 py-2 mt-2 hover:bg-blue-700">
              See Detail
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>


</template>

<style scoped>

</style>