<script setup>
import ProductCard from '../components/ProductCard.vue'

const daftarProduk = [
 { id: 1, nama: 'Kaos', harga: 250000, warna: 'bg-blue-600', gambar : '/images/kaos.jpeg' },
 { id: 2, nama: 'Hoodie', harga: 752000, warna: 'bg-orange-500', gambar : '/images/hoodie.jpg' },
 { id: 3, nama: 'SlimBag', harga: 367000, warna: 'bg-green-600', gambar : '/images/slimbag.jpg' },
]
</script>
<template>
 <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 p-6">
 <ProductCard
 v-for="produk in daftarProduk"
 :key="produk.id"
 :nama="produk.nama"
 :harga="produk.harga"
 :gambar="produk.gambar"
 />
 </div>
</template>

<style scoped>
.product-page {
 max-width: 1080px;
 margin: 0 auto;
 padding: 32px 20px 64px;
 width: 100%;
}
.product-page h1 {
 margin-bottom: 24px;
}
.product-grid {
 display: grid;
 gap: 24px;
 grid-template-columns: repeat(3, minmax(0, 1fr));
 align-items: stretch;
}
@media (max-width: 768px) {
 .product-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); }
}
@media (max-width: 480px) {
 .product-grid { grid-template-columns: 1fr; }
}
</style>    