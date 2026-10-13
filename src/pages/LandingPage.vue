<template>
 <main>
    <section class="hero">
      <h1>WELCOME TO SSST</h1>
      <p>BELANJA DI STORE KAMI DI JAMIN ORIGINAL</p>
      <RouterLink to="/product" class="btn-grad">tinggal</RouterLink>
    </section>
        <div class="card">
            <div class="box">
                <span class="emote">💰</span>
                <h2>Harga Ayaan</h2>
                <p>Aman da moal totos</p>
            </div>
            <div class="box">
                <span class="emote">🚚</span>
                <h2>Bisa di anterukeun</h2>
                <p>Aman da moal totos</p>
            </div>
            <div class="box">
                <span class="emote">✅</span>
                <h2>Kualitas di jamin edans</h2>
                <p>Aman da moal totos</p>
            </div>
        </div>

         <video controls width="480" muted loop>
 <source src="/vidio/mov_bbb.mp4" type="video/mp4" />
 Browser kamu tidak mendukung pemutaran video.
 </video>
        
 </main>
</template>

<style scoped>
main {
    display: flex;
    flex-direction: column;
    gap: 5rem;
}

.hero {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 2rem;
    padding: 2rem 5rem 2rem 5rem;
    text-align: center;
    background: linear-gradient(rgb(0, 158, 250), rgb(0, 189, 189));
    color: rgb(255, 253, 255);
    border-radius: 20px;
}
.card {
    display: grid;
    grid-template-columns: repeat(3, minmax(200px, 1fr));
    gap: 2rem;
    align-items: stretch;
}

.card2 {
    display: grid;
    gap: 2rem;
    align-items: stretch;
}

.box {
   margin-top: 2rem;
   padding: 2rem 3rem;
   border-radius: 99px;
   background-color:rgb(3, 10, 15);
   color: rgb(255, 254, 254);
   font-weight: 500;
   transition: background-color 0.3s;
}


.box {
    display: flex; gap: 1rem; flex-wrap: wrap;
    flex-direction: column;
    justify-content: center;
    gap: 1rem;
    padding: 1rem;
    background-color:rgb(6, 145, 145);
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.359);
    text-align: center;
    font-size: 1rem;
}
video {
 margin-top: 16px;
 border-radius: 10px;
 display: block;
}
.emote {
    font-size: 2rem;
}
.btn-grad {
  background-image: linear-gradient(to right, #314755 0%, #26a0da 51%, #314755 100%);
}

.btn-grad {
  margin: 10px;
  padding: 15px 45px;
  text-align: center;
  text-transform: uppercase;
  transition: 0.5s;
  background-size: 200% auto;
  color: white;
  box-shadow: 0 0 20px #eee;
  border-radius: 10px;
  display: block;
  outline: none;
  border: none;
}

.btn-grad:hover {
  background-position: right center;
  color: #fff;
  text-decoration: none;
}
</style>