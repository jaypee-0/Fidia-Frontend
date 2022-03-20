<template>
    <div id="welcome" class="container-fluid d-flex justify-content-between align-items-center">
        <div>
            <h2>Welcome back, Olivia</h2>
            <p>Track, manage and forecast your customers orders.</p>
        </div>
        <div id="buttons" class="align-items-center mb-3">
            <button class="mr-1 btn welcome-buttons px-3"><img class="pr-2 mb-1" src="../assets/svg-png-icons/import.png" alt="">Import</button>
            <button class="btn bg-purple welcome-buttons px-3"><img class="pr-2 mb-1" src="../assets/svg-png-icons/add.png" alt="">Add</button>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
  .welcome-buttons {
    border: 1px solid #d0d5dd;
    border-radius: 8px;
    font-size: 14px;
    line-height: 20px;
}
.bg-purple {
    background-color: #7F56D9;
    color: white;
}
p {
    font-weight: 400;
    font-size: 16px;
    color: #667085;
    font-family: "Inter", sans-serif;
}
@media (max-width: 568px) {
  #welcome {
    flex-direction: column;
    align-items: flex-start!important;
  }
  h2 {
    font-size: 24px;
  }
  #buttons {
    justify-content: flex-end;
  }
}  

</style>