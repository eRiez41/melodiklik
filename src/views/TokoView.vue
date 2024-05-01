<template>
  <div class="home" style="background-color: #f4f1e9;">
    <NavigationMenu class="fixed-top" /> <!-- Menambahkan komponen NavigationMenu -->
    <div class="h2-background">
      <div class="container" style="margin-top: 70px;"> <!-- Tambahkan margin-top untuk memberi ruang pada h2 -->
        <h2 class="mt-4">Daftar Toko</h2> <!-- Menambahkan margin top menggunakan kelas mt-4 -->
      </div>
    </div>
  </div>
</template>

<script>
// @ adalah alias untuk /src
import NavigationMenu from '@/components/NavigationMenu.vue' // Mengimpor komponen NavigationMenu


export default {
  name: 'HomeView',
  components: {
    NavigationMenu, // Menambahkan komponen NavigationMenu

  }
}
</script>

<style scoped>
/* Gaya kustom untuk komponen */
.h2-background {
  background-color: #b1d182; /* Warna latar belakang untuk h2 */
  padding: 10px; /* Padding agar tulisan tidak menempel pada tepi */
}
</style>
