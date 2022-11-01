<template>
    <div class="container">
        <div class="container">
            <header class="header">
                <div class="hero">
                    <img src="https://t4.ftcdn.net/jpg/01/19/25/79/360_F_119257979_B3B8wWeNZO3J9YoRT0updssvsMhcnTCo.jpg" alt="">
                </div>
            </header>
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
const nav = document.querySelector('nav ul')

        menuToggle.addEventListener('click', function () {
            nav.classList.toggle('slide')
        })
</script>

<script>
export default {
    name: 'home'
}
</script>