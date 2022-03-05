<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-none">
    <div class="container-fluid px-0">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item active">
            <NuxtLink to="/" class="nav-link"
              ><button class="px-3 btn upgrade purple">
                All time<img class="pl-2 pb-1" src="~assets/svg-png-icons/x.png" alt="" /></button
              ><span class="sr-only">(current)</span></NuxtLink
            >
          </li>
          <li class="nav-item active">
            <NuxtLink to="/" class="nav-link"
              ><button class="px-3 btn upgrade purple">
                US, AU, +4<img class="pl-2 pb-1" src="~assets/svg-png-icons/x.png" alt="" /></button
              ><span class="sr-only">(current)</span></NuxtLink
            >
          </li>
          <li class="nav-item active">
            <NuxtLink to="/" class="nav-link"
              ><button class="px-3 btn upgrade">
                <img class="pr-2 pb-1" src="~assets/svg-png-icons/filter.png" alt="" />More filters</button
              ><span class="sr-only">(current)</span></NuxtLink
            >
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
.purple {
    color: #6941C6;
    background-color: #F9F5FF;
}
.upgrade {
  border: 1px solid #d0d5dd;
  border-radius: 8px;
  font-size: 14px;
  line-height: 20px;
  font-weight: 500;
  align-items: center;
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
@media (max-width: 798px) {
  .search-icon input {
    flex-direction: row;
  width: 100%;
  }
}
</style>