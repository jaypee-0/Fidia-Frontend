<template>
  <div class="container-xl">
    <Nav />
    <Nav2nd />
    <div class="my-4">
      <Welcome />
    </div>
    <div class="d-flex flex-column flex-md-row mb-3 justify-content-between px-3">
        <Dashboard
          v-for="dashboard in dashboards"
          :key="dashboard.id" 
          :dashboard="dashboard"
        />
    </div>    
    <SearchParameters />
    <DashboardDisplay />
    <CompanyList />
  </div>
</template>

<script>
import { dashboardSection } from "@/assets/data.js";

export default {
  data() {
    return {
      dashboards: dashboardSection
    }
  }
};
</script>

<style scoped>
  @media (min-width: 1440px) {
    .container-xl{
      max-width: 1300px;
    }
  }
  @media (max-width: 320px) {
    .container-xl {
      padding: 0px;
    }
  }
  
</style>