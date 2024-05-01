<template>
    <div class="pembeli">
      <NavigationMenu /> <!-- Menambahkan komponen NavigationMenu -->
      <HelloWorld msg="Halaman Pembeli"/>
    </div>
  </template>
  
  <script>
  // @ adalah alias untuk /src
  import NavigationMenu from '@/components/NavigationMenu.vue' // Mengimpor komponen NavigationMenu
  import HelloWorld from '@/components/HelloWorld.vue'
  
  export default {
    name: 'PembeliView',
    components: {
      NavigationMenu, // Menambahkan komponen NavigationMenu
      HelloWorld
    }
  }
  </script>
  