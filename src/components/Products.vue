<template>
  <div class=" mt-4">
    <div class="text-center text-gray-800 text-2xl w-full">
      Nos spécialités
    </div>
    <div class="w-full container mx-auto lg:flex">
      <div class="bg-white rounded-lg border w-1/3 overflow-hidden my-2 mx-2 h-88 shadow-xl" v-for="(speciality, index) in specialities" :key="index">
        <img :src="speciality.image" :alt="speciality.title" class="w-full h-64 object-cover object-center">
        <div class="p-6 text-gray-800 text-lg font-semibold antialiased uppercase tracking-wide">{{speciality.description}}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Products",
  data(){
    return {
      specialities: [
        {title: 'bread', image: require('../assets/img/bread.jpg'), description: 'Pain conçu pour votre santé!'},
        {title: 'croissant', image: require('../assets/img/croissant.jpg'), description: "Croissants remplis d'épanouissement!"},
        {title: 'cake', image: require('../assets/img/cake.jpg'), description: 'Gateaux pleins de joie!'}
      ]
    }
  }
}
</script>

<style scoped>

</style>