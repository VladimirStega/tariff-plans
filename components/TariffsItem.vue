<script setup> 
  import { ref } from 'vue'
  import TariffPlanCardItem from './TariffPlanCardItem.vue'

  const tariffs = ref([
  {
    id: 1,
    title: 'Тариф Стандарт',
    description: 'Изучайте продукт и используйте его для небольшой команды',
    price: '1 200',
    services: ['Услуга 1', 'Услуга 2', 'Услуга 3', 'Услуга 4']
  },
  {
    id: 2,
    title: 'Тариф Стандарт',
    description: 'Изучайте продукт и используйте его для небольшой команды',
    price: '1 200',
    services: ['Услуга 1', 'Услуга 2', 'Услуга 3', 'Услуга 4', 'Услуга 5']
  },
  {
    id: 3,
    title: 'Тариф Стандарт',
    description: 'Изучайте продукт и используйте его для небольшой команды',
    price: '1 200',
    services: ['Услуга 1', 'Услуга 2', 'Услуга 3', 'Услуга 4', 'Услуга 5', 'Услуга 6']
  },
  {
    id: 4,
    title: 'Тариф Стандарт',
    description: 'Изучайте продукт и используйте его для небольшой команды',
    price: '1 200',
    services: ['Услуга 1', 'Услуга 2', 'Услуга 3', 'Услуга 4', 'Услуга 5', 'Услуга 6','Услуга 7']
  }
])
</script>

<template>
  <TariffPlanCardItem 
    v-for="tariff in tariffs" 
    :key="tariff.id"
    :title="tariff.title"
    :description="tariff.description"
    :price="tariff.price"
    :services="tariff.services"
  ></TariffPlanCardItem>
</template>