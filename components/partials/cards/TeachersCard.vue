<template>
  <div class="TeachersCard">
    <div>
      <b-row cols="12">
        <b-col md="6" lg="6" xl="6">
          <div>
            <img :src="require('@/assets/img/girl_3.png')" alt="girl-teach" />
          </div>
        </b-col>
        <b-col>
          <div md="6" lg="6" xl="6" class="text-md-left">
            <h3>Nombre y Apellidos</h3>
            <h2>CARGO</h2>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem,
              necessitatibus maiores consequuntur aperiam pariatur doloribus
              repudiandae explicabo, cumque optio eveniet voluptates, deserunt
              aut hic. Asperiores veritatis voluptatibus neque debitis magnam
              sint et blanditiis enim vitae molestiae ad commodi ratione fuga,
              pariatur repellendus reiciendis, aperiam maiores officia quam
              repellat. Sequi, unde?
            </p>
          </div>
        </b-col>
      </b-row>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TeachersCard',
}
</script>
