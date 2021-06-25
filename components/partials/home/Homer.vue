<template>
  <div class="Home">
    <b-container>
      <b-row>
        <b-col md="6" class="text-md-left">
          <h1>
            Incríbete ya a nuestras <br />
            clases online
          </h1>
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. <br />
            Rem possimus voluptate officia ducimus doloremque mollitia <br />
            ut a consectetur eligendi in.
          </p>
          <b-button class="px-4" pill>Ver más</b-button>
        </b-col>
        <b-col md="6" class="text-center">
          <div>
            <img
              :src="require('@/assets/img/group_people.png')"
              class="mx-auto d-block img-fluid"
              alt="group-people"
            />
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: 'Homer',
}
</script>

<style lang="css">
.Home {
  background-color: #6dadef;
  min-height: 500px;
  border-radius: 0 0 0 200px;
}
</style>
