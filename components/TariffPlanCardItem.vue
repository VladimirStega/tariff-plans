<script setup>
  defineProps(['title', 'description', 'price', 'services'])
</script>

<template>
    <div class="container">
      <div class="details" >
          <h3 class="title">
              <div>{{ title }}</div>
          </h3>
          <div class="description">{{ description }}</div>
          <div class="price">{{ price }}</div>
      </div>
      <div class="list-services">
        <div class="services">
            {{ services }}
        </div>
      </div>
        <button class="btn-tariff-card">Выбрать этот тариф</button>
    </div>
</template>



<style scoped>
  .container{
    padding: 24px;
    border: 1px solid #EAECF0;
    border-radius: 8px;
    flex-direction: column;
    align-items: flex-start;
  }

  .container:hover {
    background: radial-gradient(131.82% 103.90% at 28.14% 5.10%, rgba(251, 213, 254, 0.80) 10.57%, #FEFFD9 63.61%, #FFF 100%);
  }

  .details {
    border-bottom: 1px solid #EAECF0;
  }

  .title {
    margin: 0;
    font-size: 24px;
    font-weight: 500;
  }

  .description {
    margin-bottom: 48px;
    font-size: 16px;
    color: #667085;
  }

  .price {
    font-size: 18px;
    color: #667085;
  }

  .btn-tariff-card {
    padding: 10px 18px;
    border: 1px solid #EAECF0;
    border-radius: 8px;
    font-size: 16px;
    background: #ffffff;
  }
</style>