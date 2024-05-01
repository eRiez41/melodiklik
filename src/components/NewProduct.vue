<template>
    <div>
      <h2>New Product</h2>
      <!-- Tabel untuk menampilkan daftar produk baru -->
      <table class="table table-striped">
        <thead>
          <tr>
            <th scope="col">No</th>
            <th scope="col">Nama Barang</th>
            <th scope="col">Toko</th>
          </tr>
        </thead>
        <tbody>
          <!-- Gunakan v-for untuk menampilkan data produk -->
          <tr v-for="(product, index) in products" :key="product.id">
            <td>{{ index + 1 }}</td>
            <td>{{ product.name }}</td>
            <td>{{ product.store }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </template>
  
  <script>
  export default {
    name: 'NewProduct',
    data() {
      return {
        // Data dummy untuk produk
        products: [
          { id: 1, name: 'Product 1', store: 'Store A' },
          { id: 2, name: 'Product 2', store: 'Store B' },
          { id: 3, name: 'Product 3', store: 'Store C' },
        ]
      };
    }
  }
  </script>
  
  <style scoped>
  /* Gaya kustom untuk komponen */
  .table {
    width: 100%;
    border-collapse: collapse;
  }
  
  .table th, .table td {
    padding: 8px;
    text-align: left;
    border-bottom: 1px solid #ddd;
  }
  
  .table-striped tbody tr:nth-child(odd) {
    background-color: #f2f2f2;
  }
  </style>
  