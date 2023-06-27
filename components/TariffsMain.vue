<script setup>
  import TariffPlanCardItem from './TariffPlanCardItem.vue'
</script>

<template>
    <header>
      <div class="container">
        <TheHeader />
      </div>
      <hr>
    </header>

    <main>
      <div class="container">
        <div class="wrapper">
          <h2>Тарифные планы</h2>
          <select v-model="selected">
          </select>
        </div>
        <TariffPlanCardItem />
      </div>
    </main>
</template>

<style scoped>
    .container {
        margin: 0 auto;
        max-width: 1600px;

    }

    .wrapper {
      display: flex;
      place-items: center;
      justify-content: space-between;
    }
</style>