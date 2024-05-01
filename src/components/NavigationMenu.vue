<template>
    <nav class="navbar navbar-expand-lg navbar-dark bg-success">
      <div class="container-fluid">
        <router-link to="/" class="navbar-brand">MelodiKlik</router-link>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo02" aria-controls="navbarTogglerDemo02" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <form class="d-flex">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <router-link to="/" class="nav-link" aria-current="page">Home</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/TokoView" class="nav-link">Toko</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/PembeliView" class="nav-link">User</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/user" class="nav-link"></router-link>
            </li>
          </ul>
          <button class="btn btn-outline-light border-0" type="button">
            <i class="fas fa-user"></i> <!-- Ikon Font Awesome untuk pengguna -->
          </button>
        </form>
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'NavigationMenu'
  }
  </script>
  
  <style scoped>
  /* Tambahkan gaya kustom di sini jika diperlukan */
  .btn {
    padding: 10px 20px; /* Atur ukuran tombol */
  }
  </style>
  