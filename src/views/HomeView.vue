<template>
  <div class="home" style="background-color: #f4f1e9;">
    <NavigationMenu class="fixed-top" /> <!-- Menambahkan komponen NavigationMenu -->
    <div class="h2-background">
      <div class="container" style="margin-top: 70px;"> <!-- Tambahkan margin-top untuk memberi ruang pada h2 -->
        <h2 class="mt-4">Dashboard</h2> <!-- Menambahkan margin top menggunakan kelas mt-4 -->
      </div>
    </div>
    <div class="container"> <!-- Container untuk konten utama -->
      <div class="row">
        <div class="col-md-12">
          <SummaryWidget /> <!-- Menambahkan komponen SummaryWidget -->
        </div>
      </div>
      <div class="row mt-4">
        <div class="col-md-6">
          <NewProduct /> <!-- Menambahkan komponen NewProduct -->
        </div>
        <div class="col-md-6">
          <StatisticUser /> <!-- Menambahkan komponen StatisticUser -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ adalah alias untuk /src
import NavigationMenu from '@/components/NavigationMenu.vue' // Mengimpor komponen NavigationMenu
import SummaryWidget from '@/components/SummaryWidget.vue' // Mengimpor komponen SummaryWidget
import NewProduct from '@/components/NewProduct.vue' // Mengimpor komponen NewProduct
import StatisticUser from '@/components/StatisticUser.vue' // Mengimpor komponen StatisticUser

export default {
  name: 'HomeView',
  components: {
    NavigationMenu, // Menambahkan komponen NavigationMenu
    SummaryWidget, // Menambahkan komponen SummaryWidget
    NewProduct, // Menambahkan komponen NewProduct
    StatisticUser // Menambahkan komponen StatisticUser
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
