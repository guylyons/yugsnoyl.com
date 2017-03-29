<template>
    <main>
        <header>
            <h1>Guy Lyons</h1>
            <h2>Dev &amp; Design</h2>
            <img src="//placehold.it/180x180" alt="Guy Lyons">
        </header>
        <div class="row">
            <ul>
                <li><a href="#">Github</a></li>
                <li><a href="#">Twitter</a></li>
                <li><a href="#">LinkedIn</a></li>
                <li><a href="#">Email</a></li>
            </ul>
        </div>
    </main>
</template>

<script>
import Header from '../components/Header.vue'
import Footer from '../components/Footer.vue'

export default {
    data: () => {
        return { name: 'world' }
    },
    components: {
        Header,
        Footer
    }
}
</script>
