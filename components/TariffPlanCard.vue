<template>
  <div class="container">
    <TariffPlanCardItem>
      <template #title>Тариф Стандарт</template>
      <template #description>
        Изучайте продукт и используйте его для небольшой команды
      </template>
          
      <template #price><span class="prise-style">1 200 &#8381;</span> /месяц</template>
      <div class="services">
        1
      </div>
    </TariffPlanCardItem>

    <TariffPlanCardItem>
      <template #title>Тариф Про</template>
      <template #description>
        Изучайте продукт и используйте его для небольшой команды
      </template>
          
      <template #price><span class="prise-style">2 200 &#8381;</span> /месяц</template>
      <div class="services">
        1
      </div>
    </TariffPlanCardItem>

    <TariffPlanCardItem>
      <template #title>Тариф Премиум</template>
      <template #description>
        Изучайте продукт и используйте его для небольшой команды
      </template>
          
      <template #price><span class="prise-style">4 700 &#8381;</span> /месяц</template>
      <div class="services">
        1
      </div>
    </TariffPlanCardItem>

    <TariffPlanCardItem>
      <template #title>Тариф Максимум</template>
      <template #description>
        Изучайте продукт и используйте его для небольшой команды
      </template>
          
      <template #price><span class="prise-style">10 500 &#8381;</span> /месяц</template>
      <div class="services">
        1
      </div>
    </TariffPlanCardItem>
  </div>
</template>

<style scoped>
  .container {
    display: flex;
    gap: 24px;
  }

  .prise-style {
    font-size: 48px;
    font-weight: 600;
    line-height: 64px;
    color: #0D1421;
  }
</style>