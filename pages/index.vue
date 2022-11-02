<template>
    <div class="container">
      <navbar/>
        <div class="container">
            <header class="header">
                <div class="hero">
                    <img src="https://t4.ftcdn.net/jpg/01/19/25/79/360_F_119257979_B3B8wWeNZO3J9YoRT0updssvsMhcnTCo.jpg" alt="">
                </div>
            </header>
            <section class="cards">
                 <div v-for="product in products.data" :key = "product.id" class="card">
                     <nuxt-link :to="'product/'+product.id">
                        <div class="icon">
                            <img :src="product.picture" alt="">
                        </div>
                        <h3>{{product.name}}</h3>
                     </nuxt-link>
                    
                </div>
                
            </section>

        </div>
    </div>
</template>



<script>
import axios from 'axios'
export default {
    name: 'home',
    data() {
        return{
            products:[]
        }
    },
    
  methods: {
        async getData() {
            await axios
            .get("https://my-json-server.typicode.com/rofinurhakim/test.json/posts" )
            .then((res) => {
            this.products = res;
        });
        },
  },

  mounted() {
      this.getData()
  },

}
</script>