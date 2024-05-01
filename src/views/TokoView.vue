<template>
    <div class="toko">
      <NavigationMenu /> <!-- Menambahkan komponen NavigationMenu -->
      <HelloWorld msg="Halaman Toko"/>
    </div>
  </template>
  
  <script>
  // @ adalah alias untuk /src
  import NavigationMenu from '@/components/NavigationMenu.vue' // Mengimpor komponen NavigationMenu
  import HelloWorld from '@/components/HelloWorld.vue'
  
  export default {
    name: 'TokoView',
    components: {
      NavigationMenu, // Menambahkan komponen NavigationMenu
      HelloWorld
    }
  }
  </script>
  