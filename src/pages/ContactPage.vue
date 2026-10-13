
<template>
    <div class="Judul">
      <h1>Kontak Kami</h1>
      </div>
  <div class="contact-container">

    <!-- BAGIAN KIRI -->
    <div class="info-kontak">
      <h1>Info kontak</h1>

      <h2>Alamat</h2>
      <p>Gak tau kemana</p>

      <h2>Telepon</h2>
      <p>(+62)89635605617</p>

      <h2>Email</h2>
      <p>SMKYASOR@gmail.com </p>
    </div>

    <!-- BAGIAN KANAN -->
    <div class="form-kontak">
      <h1>Kirim Pesan</h1>

      <form @submit="kirimPesan">

        <label>Nama</label>
        <input
        type="text"
        placeholder="Masukkan Nama"
        required
        >

        <label>Email</label>
        <input
        type="email"
        placeholder="Masukan Email"
        required
        pattern="[a-zA-Z0-9._%+-]+@gmail\.com"
        title="Email harus menggunakan @gmail.com"
        >

        <label>Pesan</label>
        <textarea
        placeholder="Masukkan Pesan"
        required
        ></textarea>

        <button type="submit">Kirim</button>

      </form>
    </div>

  </div>
</template>
        <script setup>
        function kirimPesan(event) {
          event.preventDefault()
        
          alert("Pesan berhasil dikirim!")
        
          // Reset / refresh halaman
          window.location.reload()
        }
        </script>

<style scoped>
.Judul {
  text-align: center;
  padding: 40px;
   background: linear-gradient(rgb(0, 158, 250), rgb(0, 189, 189));
  color: white;
}
.contact-container {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  width: 100%;
  padding: 30px 50px;
  box-sizing: border-box;
}

/* KIRI */
.info-kontak {
  width: 45%;
}

/* KANAN */
.form-kontak {
  width: 45%;
}

/* Supaya form berada di tengah area kanan */
.form-kontak form {
  display: flex;
  flex-direction: column;
  width: 300px;
}

.form-kontak input,
.form-kontak textarea {
  width: 100%;
  padding: 8px;
  margin-bottom: 8px;
  box-sizing: border-box;
}

.form-kontak textarea {
  height: 80px;
}

.form-kontak button {
  width: fit-content;
  padding: 5px 15px;
  align-self: center;
}
</style>