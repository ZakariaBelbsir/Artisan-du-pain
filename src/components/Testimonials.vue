<template>
 <div class="mt-4">
   <div class="text-center text-gray-800 text-2xl w-full">
     Ce que nos clients disent
   </div>
   <div class="w-full container mx-auto lg:flex">
     <div class="bg-white rounded-lg border overflow-hidden h-32 lg:w-2/3 my-2 mx-2 shadow-xl" v-for="(testimony, index) in testimonies" :key="index">
       <div class="p-6 text-gray-800 text-lg font-semibold antialiased uppercase tracking-wide">
         "{{testimony.clientReview}}" <br>
         <span> - {{testimony.clientName}}</span>
       </div>
     </div>
   </div>
 </div>
</template>

<script>
export default {
  name: "Testimonials",
  data(){
    return {
      testimonies: [
        {'clientName': 'John Doe', 'clientReview': "«Je ne me suis jamais senti aussi satisfait de manger que du pain»"},
        {'clientName': 'Jane Doe', 'clientReview': "après avoir pris ma première bouchée, je me suis dit si seulement cela n'est jamais fini!"}
      ]
    }
  }
}
</script>

<style scoped>

</style>