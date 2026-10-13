<script setup>
defineProps({
  nama: {
    type: String,
    required: true,
  },
  jabatan: {
    type: String,
    required: true,
  },
  inisial: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <article class="team-card">
    <div class="avatar" aria-hidden="true">{{ inisial }}</div>
    <h3>{{ nama }}</h3>
    <p>{{ jabatan }}</p>
  </article>
</template>

<style scoped>
.team-card {
  width: 180px;
  padding: 24px 16px;
  border: 1px solid var(--border);
  border-radius: var(--radius);
  background: var(--bg-soft);
  text-align: center;
}

.avatar {
  display: grid;
  width: 64px;
  height: 64px;
  margin: 0 auto 16px;
  place-items: center;
  border-radius: 50%;
  background: var(--gradient-header);
  color: #fff;
  font-size: 1.5rem;
  font-weight: 700;
}

.team-card h3 {
  margin: 0 0 8px;
}

.team-card p {
  margin: 0;
  color: var(--text-muted);
}
</style>
