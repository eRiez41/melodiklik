<template>
  <div class="summary-widget-container">
    <div class="row">
      <div class="col-md-3">
        <div class="card" style="background-color: #ff9800; color: #fff;">
          <div class="card-body">
            <h5 class="card-title"><i class="fas fa-store" style="color: #fff;"></i> Total Toko</h5>
            <p class="card-text">{{ totalStores }}</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card" style="background-color: #2196f3; color: #fff;">
          <div class="card-body">
            <h5 class="card-title"><i class="fas fa-box" style="color: #fff;"></i> Total Barang</h5>
            <p class="card-text">{{ totalProducts }}</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card" style="background-color: #4caf50; color: #fff;">
          <div class="card-body">
            <h5 class="card-title"><i class="fas fa-users" style="color: #fff;"></i> Total User</h5>
            <p class="card-text">{{ totalUsers }}</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card" style="background-color: #f44336; color: #fff;">
          <div class="card-body">
            <h5 class="card-title"><i class="fas fa-user-check" style="color: #fff;"></i> Pengguna Aktif</h5>
            <p class="card-text">{{ totalActive }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SummaryWidget',
  data() {
    return {
      totalStores: 0,
      totalProducts: 0,
      totalUsers: 0,
      totalActive: 0
    };
  },
  // Logika komponen
  mounted() {
    // Ambil data dari API atau sumber lainnya untuk mendapatkan total toko, barang, dan user
    // Di sini, saya menggunakan data dummy
    this.totalStores = 10; // Misalnya, 10 toko
    this.totalProducts = 150; // Misalnya, 150 barang
    this.totalUsers = 500; // Misalnya, 500 user
    this.totalActive = 120; // Misalnya, 500 user
  }
}
</script>

<style scoped>
/* Gaya kustom untuk komponen */
.summary-widget-container {
  margin-top: 20px;
}
</style>
