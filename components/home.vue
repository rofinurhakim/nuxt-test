<template>
    <div class="container">
        <div class="container">
            <header class="header">
                <div class="hero">
                    <img src="https://t4.ftcdn.net/jpg/01/19/25/79/360_F_119257979_B3B8wWeNZO3J9YoRT0updssvsMhcnTCo.jpg" alt="">
                </div>
                <div class="features features-1">
                    <h4>hahah</h4>
                    <p>asnaj</p>
                </div>
                <div class="features features-2">
                    <h4>hahah</h4>
                    <p>asnaj</p>
                </div>
            </header>

            <nav class="menu">
                <div class="menu-toggle">
                    <input type="checkbox">
                    <span></span>
                    <span></span>
                    <span></span>
                </div>
                <div class="brand">
                    <h1>Japanese Food</h1>
                </div>
                <ul class="menu-list">
                    <li><a href="">Menu</a></li>
                    <li><a href="">Product</a></li>
                    <li><a href="">Menu</a></li>
                    <li><a href="">Product</a></li>
                </ul>
            </nav>

            <section class="cards">
                <div class="card">
                    <div class="icon"></div>
                    <h3>Ramen</h3>
                    <p>lorem ipsum dimsum</p>
                </div>
                <div class="card">
                    <div class="icon"></div>
                    <h3>Ramen</h3>
                    <p>lorem ipsum dimsum</p>
                </div>
                <div class="card">
                    <div class="icon"></div>
                    <h3>Ramen</h3>
                    <p>lorem ipsum dimsum</p>
                </div>
                <div class="card">
                    <div class="icon"></div>
                    <h3>Ramen</h3>
                    <p>lorem ipsum dimsum</p>
                </div>
                <div class="card">
                    <div class="icon"></div>
                    <h3>Ramen</h3>
                    <p>lorem ipsum dimsum</p>
                </div>
            </section>
        </div>
    </div>
</template>

<script>
const menuToggle = document.querySelector('.menu-toggle')
const nav = document.querySelector('nav,ul')

        menuToggle.addEventListener('click', function () {
            nav.classList.toggle('slide')
        })


</script>

<script>
export default {
    name: 'home'
}
</script>