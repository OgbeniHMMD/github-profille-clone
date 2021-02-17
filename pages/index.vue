<template>
  <main>
    <partials-app-bar />
    <partials-nav-bar />

    <section class="container main-section">
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
  width: 25%;
}

.main {
  width: 75%;
}
</style>
