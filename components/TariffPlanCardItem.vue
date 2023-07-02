<script>
import IconCheck from './icons/IconCheck.vue'
export default {
  components: { IconCheck },
  props: ["title", "description", "price", "services"]
}
</script>

<template>
    <div class="container">
      <div class="details">
        <h3 class="title">
          {{ title }}
        </h3>
        <p class="description">
          {{ description }}
        </p>
        <p class="price">
          <span class="prise-style">{{ price }} &#8381;</span> /месяц
        </p>
        <ul class="list-services">
          <li class="services"
            v-for="service in services" 
            :key="service.id">
             <IconCheck class="icon-check"/> {{ service.item }}
          </li>
        </ul>
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

  .title {
    margin: 0;
    font-size: 24px;
    font-weight: 500;
  }

  .description {
    margin-bottom: 48px;
    margin-right: 40px;
    font-size: 16px;
    color: #667085;
  }

  .price {
    margin-bottom: 24px;
    padding-bottom: 24px;
    font-size: 18px;
    color: #667085;
    border-bottom: 1px solid #EAECF0;
  }

  .prise-style {
    font-size: 48px;
    font-weight: 600;
    line-height: 64px;
    color: #0D1421;
  }

  .list-services {
    padding: 0;
  }

  .services {
    display: flex;
    place-items: center;
    list-style-type: none;
    padding-bottom: 16px;
  }

  .icon-check {
    margin-right: 16px;
  }

  .btn-tariff-card {
    padding: 10px 18px;
    border: 1px solid #EAECF0;
    border-radius: 8px;
    font-size: 16px;
    background: #ffffff;
  }
</style>