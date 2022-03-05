<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-none">
    <div class="container-fluid px-0">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <NuxtLink class="nav-link active" to="/">Overview</NuxtLink>
        </li>
        <li class="nav-item">
          <NuxtLink class="nav-link active" to="/">Notifications</NuxtLink>
        </li>
        <li class="nav-item">
          <NuxtLink class="nav-link active" to="/">Analytics</NuxtLink>
        </li>
        <li class="nav-item">
          <NuxtLink class="nav-link active" to="/">Saved reports</NuxtLink>
        </li>
        <li class="nav-item">
          <NuxtLink class="nav-link active" to="/">Trade history</NuxtLink>
        </li>
        <li class="nav-item">
          <NuxtLink class="nav-link active" to="/">User reports</NuxtLink>
        </li>
      </ul>
      <form class="d-flex ml-auto">
        <div class="search-icon">
          <input
            class="form-control me-2"
            type="search"
            placeholder="Search"
            aria-label="Search"
          />
        </div>
      </form>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style scoped>
@media (max-width: 1024px) {
  nav {
    display: none;
  }
}
.navbar ul li {
  font-size: 16px;
  color: #344054;
    font-weight: 400;
}
.search-icon input {
  padding-left: 30px;
  background-image: url("~assets/svg-png-icons/search.svg");
  background-size: 16px 16px;
  background-repeat: no-repeat;
  background-position: 10px 0.6rem;
  border-radius: 8px;
  width: 320px;
}
</style>