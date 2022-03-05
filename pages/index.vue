<template>
  <div class="container ">
    <Nav />
    <Nav2nd />
     <div class="d-flex mb-5 justify-content-between px-3">
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
    .container {
      max-width: 1300px;
    }
  }
  
</style>