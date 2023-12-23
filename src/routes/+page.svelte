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
    @import url('https://fonts.googleapis.com/css2?family=Kalnia:wght@500&family=Montserrat:wght@100&family=Playfair:opsz,wght@5..1200,300&family=Quicksand:wght@500&display=swap');


    /* fit later the overflow issue in landing */
    :global(body) {
        font-family: 'Playfair', serif;
        background-color: #fafafa;
        margin: 0px;
    }

    main {
        display: flex;
        flex-direction: column;
        max-width: 100%; /* Ensure it doesn't exceed the viewport width */
        margin: 0; /* Center the container horizontally */
    }
</style>