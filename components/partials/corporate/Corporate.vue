<template>
  <div class="Corporate">
    <BannerTop :image="image" />
    <b-container>
      <div>
        <div>
          <h3 class="Corporate-title">Corporativo</h3>
          <p class="Corporate-paragraph">
            La inversión en capacitación se recupera con creces y se traduce en
            aprender a retener clientes, incrementar ventas, rentabilizar mejor
            la infraestructura instalada y elevar el grado de compromiso de los
            empleados con la marca que representan. <br />
            Nos ajustamos a su tiempo y presupuesto para impartir nuestra
            capacitación.
          </p>
        </div>
        <div>
          <div v-for="item in data" :key="item.title">
            <CorporateCard :item="item" />
          </div>
        </div>
      </div>
    </b-container>
  </div>
</template>

<script>
import BannerTop from '~/components/common/BannerTop.vue'
import CorporateCard from '~/components/partials/cards/CorporateCard.vue'
export default {
  name: 'Corporate',
  components: { BannerTop, CorporateCard },
  data() {
    return {
      image: require('@/assets/img/banner/corporativo.jpg'),
      data: [
        {
          image: require('@/assets/img/corporate/Group1.png'),
          title: 'Televentas',
          style: 'background-color: #FFE2D7; height: 218px; width: 383px;',
          paragraph:
            'Creado para un grupo determinado de integrantes, cumpliendo con todos nuestros estándares. Nos reinventamos para ustedes y les brindamos un programa 100% ONLINE con clases totalmente en vivo pensando en un momento de aprendizaje e integración con tus compañeros.',
        },
        {
          image: require('@/assets/img/corporate/Group2.png'),
          title: 'Atención al cliente',
          style: 'background-color: #D2E7FF; height: 218px; width: 383px;',
          paragraph:
            'Creado para un grupo determinado de integrantes, cumpliendo con todos nuestros estándares. Nos reinventamos para ustedes y les brindamos un programa 100% ONLINE con clases totalmente en vivo pensando en un momento de aprendizaje e integración con tus compañeros.',
        },
        {
          image: require('@/assets/img/corporate/Group3.png'),
          title: 'Gestión de reclamos',
          style: 'background-color: #FFE486; height: 218px; width: 383px;',
          paragraph:
            'Creado para un grupo determinado de integrantes, cumpliendo con todos nuestros estándares. Nos reinventamos para ustedes y les brindamos un programa 100% ONLINE con clases totalmente en vivo pensando en un momento de aprendizaje e integración con tus compañeros.',
        },
      ],
    }
  },
}
</script>

<style>
.Corporate-title {
  font-weight: bold;
  font-size: 40px;
  line-height: 60px;
  color: #4a90e2;
}
.Corporate-paragraph {
  font-weight: normal;
  font-size: 21px;
  line-height: 31px;
  color: #000;
}
</style>
