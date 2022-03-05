<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-none">
    <div class="container-fluid px-0">
      <NuxtLink class="navbar-brand" to="/"
        ><img src="~assets/svg-png-icons/content.png" alt="" /> Untitled
        UI</NuxtLink
      >
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <NuxtLink class="nav-link active" to="/">Home</NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink class="nav-link active" to="/">Dashboard</NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink class="nav-link active" to="/">Projects</NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink class="nav-link active" to="/">Tasks</NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink class="nav-link active" to="/">Reporting</NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink class="nav-link active" to="/">Users</NuxtLink>
          </li>
        </ul>

        <ul class="navbar-nav ml-auto align-items-center">
          <li class="nav-item active">
            <NuxtLink to="/" class="nav-link"
              ><button class="px-4 btn upgrade">
                <img src="~assets/svg-png-icons/zap.png" alt="" /> Upgrade now</button
              ><span class="sr-only">(current)</span></NuxtLink
            >
          </li>
          <li class="nav-item active">
            <NuxtLink to="/" class="nav-link"
              ><img src="~assets/svg-png-icons/setting.png" alt="" /><span
                class="sr-only"
                >(current)</span
              ></NuxtLink
            >
          </li>
          <li class="nav-item active">
            <NuxtLink to="/" class="nav-link"
              ><img src="~assets/svg-png-icons/notification.png" alt="" /><span
                class="sr-only"
                >(current)</span
              ></NuxtLink
            >
          </li>
          <li class="nav-item active">
            <NuxtLink to="/" class="nav-link"
              ><img src="~assets/images/Avatar-1.png" alt="" /><span
                class="sr-only"
                >(current)</span
              ></NuxtLink
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style scoped>
.navbar .nabarbrand {
  color: #101828;
  font-weight: 900;
}

.navbar ul li {
  font-size: 16px;
}
.upgrade {
  border: 1px solid #d0d5dd;
  border-radius: 8px;
  font-size: 14px;
  line-height: 20px;
}
li {
  font-weight: 400;
}
</style>