<template>
  <div class="CorporateCard">
    <b-card no-body class="overflow-hidden my-5">
      <b-row no-gutters>
        <b-col md="4">
          <b-card-img
            :style="item.style"
            :src="item.image"
            alt="Image"
            class="rounded-0"
          ></b-card-img>
        </b-col>
        <b-col md="8">
          <b-card-body :title="item.title">
            <b-card-text>
              {{ item.paragraph }}
            </b-card-text>
          </b-card-body>
        </b-col>
      </b-row>
    </b-card>
  </div>
</template>

<script>
export default {
  name: 'CorporateCard',
  props: {
    item: {
      type: Object,
      default() {
        return {
          title: 'Horizontal Card',
          paragraph:
            "There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable. If you are going to use a passage of Lorem Ipsum, you need to be sure there isn't anything embarrassing hidden.",
          image: 'https://picsum.photos/400/400/?image=20',
          style: 'background-color: #FAFAFA; max-height: 218px;',
        }
      },
    },
  },
}
</script>
