<template>
  <div class="md:flex flex-col w-screen h-screen content-center p-6">
    <NavBar />
    <Nuxt />
    <div hidden id="snipcart" :data-api-key="apiKey"></div>
  </div>
</template>

<script>
  import NavBar from '@/components/NavBar.vue'
  export default {
    name: 'default',
    data() {
      return {
        apiKey: process.env.SNIPCART_API_KEY || "NWE5OWVhMjYtYTNmMi00MWE1LWFkMzMtYWMwNTk5ZjJlZDFiNjM3NDc2MDE2MDIzOTIyMjk2"
      }
    }

  }
</script>