<script>
    import Header from './layout/Header.svelte';
    import Footer from './layout/Footer.svelte';
    import Landing from './landing/Landing.svelte';
</script>

<Header />

<main>
    <slot>
        <!-- This is where the content of the page will go -->
        <Landing />
    </slot>
</main>

<Footer />

<style>
    :global(body) {
        font-family: 'Arial', sans-serif;
        background-color: #fafafa;
    }
</style>