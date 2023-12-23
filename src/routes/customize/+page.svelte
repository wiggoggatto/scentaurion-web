<script>
    import Header from '../layout/Header.svelte';
    import Footer from '../layout/Footer.svelte';
    import Signed from './signed/Signed.svelte';
    import Unsigned from './unsigned/Unsigned.svelte';

    let isSigned = false;
</script>

<Header />

<div>
    {#if isSigned}
        <Signed />
    {:else}
        <Unsigned />
    {/if}
</div>

<Footer />