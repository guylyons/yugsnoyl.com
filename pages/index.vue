<template>
    <main>
        <Header></Header>
        <Footer></Footer>
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
