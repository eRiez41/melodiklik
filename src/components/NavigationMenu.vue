<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-custom fixed-top">
    <div class="container-fluid">
      <router-link to="/" class="navbar-brand">MelodiKlik - {{ userLevel }}</router-link> <!-- Menampilkan level user -->
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo02" aria-controls="navbarTogglerDemo02" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <form class="d-flex">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <router-link to="/" class="nav-link" exact active-class="active" aria-current="page">Home</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/TokoView" class="nav-link" active-class="active">Toko</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/PembeliView" class="nav-link" active-class="active">User</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/user" class="nav-link" active-class="active"></router-link>
          </li>
        </ul>
        <button class="btn btn-outline-light border-0" type="button">
          <i class="fas fa-user"></i>
        </button>
      </form>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavigationMenu',
  data() {
    return {
      userLevel: 'Admin' // Variabel sementara untuk menampilkan level user
    };
  }
}
</script>

<style scoped>
.btn {
  padding: 10px 20px;
}

.bg-custom {
  background-color: #2b463c; /* Warna latar belakang navbar */
}
</style>
