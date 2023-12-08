<template>
  <nav class="navbar navbar-expand-lg bg-body-tertiary w-100">
    <div class="container-fluid">
      <router-link to="/" class="navbar-brand">AFofUK</router-link>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <router-link to="/" class="nav-link active" aria-current="page">Головна</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/gallery" class="nav-link">Галерея</router-link>
          </li>
          <li class="nav-item dropdown">
            <a href="#" class="nav-link dropdown-toggle" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              Більше
            </a>
            <ul class="dropdown-menu">
              <li><router-link to="/about" class="dropdown-item">Про нас</router-link></li>
              <li><router-link to="/contact" class="dropdown-item">Зв'язатися з нами</router-link></li>
              <li><hr class="dropdown-divider"></li>
              <li><router-link to="/" class="dropdown-item">Головна</router-link></li>
            </ul>
          </li>
        </ul>
        <form class="d-flex" role="search">
          <input class="form-control me-2" type="search" placeholder="Пошук" aria-label="Search">
          <button class="btn btn-outline-success" type="submit">Пошук</button>
        </form>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>

</style>