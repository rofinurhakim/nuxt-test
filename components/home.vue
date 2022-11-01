<template>
    <div class="container">
        <div class="container">
            <header class="header">
                <div class="hero">
                    <img src="https://t4.ftcdn.net/jpg/01/19/25/79/360_F_119257979_B3B8wWeNZO3J9YoRT0updssvsMhcnTCo.jpg" alt="">
                </div>
            </header>
            <section class="cards">
                <div v-for="product in products.data" :key = "product.id" class="card">
                    <div class="icon"></div>
                    <h3>{{product.title}}</h3>
                    <p>lorem ipsum dimsum</p>
                </div>
                
            </section>

        </div>
    </div>
</template>



<script>
export default {
    name: 'home',
    data() {
        return{
            products:[]
        }
    },
    
  methods: {
        async getData() {
            await this.$axios
            .get("https://my-json-server.typicode.com/typicode/demo/posts" )
            .then((res) => {
            this.products = res;
            console.log(this.products, 'masuk')
        });
        },
  },

  mounted() {
      this.getData()
  },

}
</script>