<template>
  <div class="home">
    <NavigationMenu /> <!-- Menambahkan komponen NavigationMenu -->
    <div class="container">
      <h2 class="mt-4">Dashboard</h2> <!-- Menambahkan margin top menggunakan kelas mt-4 -->
      <div class="row">
        <div class="col-md-12">
          <SummaryWidget /> <!-- Menambahkan komponen SummaryWidget -->
        </div>
      </div>
    </div>
  </div>
</template>


<script>
// @ adalah alias untuk /src
import NavigationMenu from '@/components/NavigationMenu.vue' // Mengimpor komponen NavigationMenu
import SummaryWidget from '@/components/SummaryWidget.vue' // Mengimpor komponen SummaryWidget


export default {
  name: 'HomeView',
  components: {
    NavigationMenu, // Menambahkan komponen NavigationMenu
    SummaryWidget, // Menambahkan komponen SummaryWidget

  }
}
</script>
