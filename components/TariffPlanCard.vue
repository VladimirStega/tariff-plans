<script>
export default {
  data() {
    return {
      tariffs: [
        { 
          id: 1, 
          title: 'Тариф Стандарт',
          description: "'Изучайте продукт и используйте его для небольшой команды'",
          price: '1 200',
          services: [
            { id: 1, item:'Услуга 1'}, 
            { id: 2, item:'Услуга 2'}, 
            { id: 3, item:'Услуга 3'}, 
            { id: 4, item:'Услуга 4'}
          ], 
        },
        { 
          id: 2, 
          title: 'Тариф Про',
          description: 'Изучайте продукт и используйте его для небольшой команды',
          price: '2 200',
          services: [
            { id: 1, item:'Услуга 1'}, 
            { id: 2, item:'Услуга 2'}, 
            { id: 3, item:'Услуга 3'}, 
            { id: 4, item:'Услуга 4'}, 
            { id: 5, item:'Услуга 5'}
          ], 
        },
        { 
          id: 3, 
          title: 'Тариф Премиум',
          description: 'Изучайте продукт и используйте его для небольшой команды',
          price: '4 700',
          services: [
            { id: 1, item:'Услуга 1'}, 
            { id: 2, item:'Услуга 2'}, 
            { id: 3, item:'Услуга 3'},
            { id: 4, item:'Услуга 4'}, 
            { id: 5, item:'Услуга 5'}, 
            { id: 6, item:'Услуга 6'}
          ], 
        },
        { 
          id: 4, 
          title: 'Тариф Максимум',
          description: 'Изучайте продукт и используйте его для небольшой команды',
          price: '10 500',
          services: [
            { id: 1, item:'Услуга 1'}, 
            { id: 2, item:'Услуга 2'}, 
            { id: 3, item:'Услуга 3'},
            { id: 4, item:'Услуга 4'}, 
            { id: 5, item:'Услуга 5'}, 
            { id: 6, item:'Услуга 6'}, 
            { id: 7, item:'Услуга 7'}
          ], 
        },
      ]
    }
  }
}
</script>

<template>
  <div class="container">
    <TariffPlanCardItem
      v-for="tariff in tariffs"
      :key="tariff.id"
      :title="tariff.title"
      :description="tariff.description"
      :price="tariff.price"
      :services="tariff.services"
	  ></TariffPlanCardItem>
  </div>

</template>

<style scoped>

  .container {
    display: flex;
    justify-content: space-between;
    gap: 24px;
  }


</style>