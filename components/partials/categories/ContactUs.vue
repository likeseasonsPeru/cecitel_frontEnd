<template>
  <div class="ContactUs">
    <b-container>
      <b-row>
        <b-col md="6">
          <div>
            <h3>Contáctanos</h3>
            <span>Elige el medio de comunicación de tu preferencia</span>
            <h6>Telefono</h6>
            <span><a href="tel:969756268">969756268</a></span>
            <h6>E-mail</h6>
            <span
              ><a href="mail:contacto@cecitel.com.pe"
                >contacto@cecitel.com.pe</a
              ></span
            >
            <div>
              <img
                :src="require('~/components/svg/icons/whatsapp.svg')"
                alt="Icon whatsapp"
              />
              971563214
            </div>
            <div>
              <img
                :src="require('~/components/svg/icons/messenger.svg')"
                alt="Icon messenger"
              />
              Facebook Messenger Cecitel
            </div>
            <h6>Síguenos</h6>
            <div class="d-flex">
              <div>
                <img
                  :src="require('~/components/svg/icons/facebook.svg')"
                  alt="Icon facebook"
                />
              </div>
              <div>
                <img
                  :src="require('~/components/svg/icons/instagram.svg')"
                  alt="Icon instagram"
                />
              </div>
            </div>
          </div>
        </b-col>
        <b-col md="6"> <ContactForm /> </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import ContactForm from '~/components/partials/forms/ContactForm.vue'
export default {
  name: 'ContactUs',
  components: { ContactForm },
}
</script>

<style>
.ContactUs {
  font-size: 18px;
}
</style>
