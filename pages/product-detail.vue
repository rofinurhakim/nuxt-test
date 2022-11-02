<template>
    <div class="small-container single-product">
        <div class="row">
            <div class="col-2">
                <img :src="product.picture">
            </div>
            <div class="col-2">
                <p>Ramen Type</p>
                <h1>{{product.name}}</h1>
                <h3>Product Detail</h3>
                <br>
                <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, </p>
            </div>
        </div>
    </div>
</template>

<script>
import '../assets/product.css'
export default {
    data() {
        return {
            product:{}
        }
    },
    methods: {
    async getDataId() {
      const _this = this;
      await this.$axios
        .get("https://my-json-server.typicode.com/rofinurhakim/test.json/posts/" + this.$route.params.id)
        .then((response) => {
          this.product = response.data;
        });
    },
    },

      mounted() {
      this.getDataId()
  },

}
</script>