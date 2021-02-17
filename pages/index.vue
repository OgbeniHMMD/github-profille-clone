<template>
  <main>
    <partials-app-bar />
    <partials-nav-bar />

    <section class="main-section">
      <repository-side-bar class="aside" />
      <repository-main-list class="main" />
    </section>

    <partials-footer />
  </main>
</template>

<style scoped>
.main-section {
  display: flex;
}

.aside {
  width: 20%;
}

.main {
  width: 80%;
}
</style>
