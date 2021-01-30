<template>
  <div class="mt-4">
    <div class="text-center text-gray-800 text-2xl w-full">
      Contactez nous
    </div>
    <div class="container my-12 flex content-center items-center">
      <form class="max-w-lg w-full mx-auto border shadow-xl rounded-lg px-4 py-2"
            action="POST" data-netlify="true"
            name="contact"
            data-netlify-honeypot="bot-field">
        <input type="hidden" name="form-name" value="contact" />
        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full px-3">
            <label class="block uppercase tracking-wide text-gray-800 text-xs font-bold mb-2" for="name">
              Nom
            </label>
            <input class="appearance-none block w-full bg-gray-200 text-gray-700 border
           border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none
           focus:bg-white focus:border-gray-500"
                   id="name" required type="text"
            name="name">
          </div>
        </div>
        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full px-3">
            <label class="block uppercase tracking-wide text-gray-800 text-xs font-bold mb-2" for="email">
              E-mail
            </label>
            <input
                class="appearance-none block w-full bg-gray-200 text-gray-700 border
              border-gray-200 rounded py-3 px-4 mb-3 leading-tight
              focus:outline-none focus:bg-white focus:border-gray-500"
                id="email" required type="email"
            name="email">
          </div>
        </div>
        <div class="flex flex-wrap -mx-3 mb-6">
          <div class="w-full px-3">
            <label class="block uppercase tracking-wide text-gray-800 text-xs font-bold mb-2" for="message">
              Message
            </label>
            <textarea class=" no-resize appearance-none block w-full bg-gray-200 text-gray-700 border
           border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none
           focus:bg-white focus:border-gray-500 h-48 resize-none"
                      required id="message"
            name="message"></textarea>
          </div>
        </div>
        <div class="">
          <div class="md:w-1/3">
            <button class="shadow bg-blue-400 hover:bg-blue-500 focus:shadow-outline
           focus:outline-none text-white font-bold py-2 px-4 rounded" type="submit">
              Envoyer
            </button>
          </div>
          <!--        <div class="md:w-2/3"></div>-->
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "Contact"
}
</script>

<style scoped>

</style>