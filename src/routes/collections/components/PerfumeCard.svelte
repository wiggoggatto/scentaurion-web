<script>
    export let show_image;
    export let fade_image;
    export let title;
    export let description;
    export let cost;
    let isHovered = false;

    function handleHover() {
        isHovered = true;
    }

    function handleMouseLeave() {
        isHovered = false;
    }
</script>

<div class="perfume-card" on:mouseenter={handleHover} on:mouseleave={handleMouseLeave}>
    {#if isHovered}
        <img src={image} alt={title} />
    {:else}
        <img src={show_image} alt={title} />
        <h3>{title}</h3>
        <p>{description}</p>
        <p>Cost: ${cost}</p>
    {/if}
</div>

<style>
    .perfume-card {
        border: 1px solid #ccc;
        padding: 10px;
        margin-bottom: 10px;
    }

    img {
        width: 100%;
        max-height: 200px;
        object-fit: cover;
        margin-bottom: 10px;
    }

    h3 {
        margin: 0;
        font-size: 18px;
    }

    p {
        margin: 0;
        font-size: 14px;
    }
</style>
