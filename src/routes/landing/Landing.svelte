
<script>
    import BentoBox from "./components/BentoBox.svelte"
</script>

<div class="container">
    <header class="header">
        <h1>Scentaurion</h1>
        <p>Tailor-made Fragrances</p>
        <br>
        <p>Insert Advertisement Here</p>
    </header>

    <div class="text">
        <h3>Latest in Scentaurion's Collection</h3>
        <h4>Girl Math Series</h4>
    </div>


    <div class="product-list">
        <div class="product-card">
            <img src="perfume1.jpg" alt="Perfume 1">
            <h2>Leofgifu</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </div>
        <div class="product-card">
            <img src="perfume2.jpg" alt="Perfume 2">
            <h2>Aethlyn</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </div>
        <div class="product-card">
            <img src="perfume3.jpg" alt="Perfume 3">
            <h2>Perfume 3</h2>
            <p>Lorem ipsum dolor sit amet, consecstetur adipiscing elit.</p>
        </div>
    </div>

    <div class="bento">
        <BentoBox/>
    </div>

    <div class="text">
        <h3>Craft Your Signature Scent</h3>
        <h4>Learn, create, and personalize your own fragrance masterpiece.</h4>
    </div>

    <div class="text">
        <h3>Sustainability and Ethical Production</h3>
        <h4>Indulge without guilt with our strict ethical production protocols.</h4>
    </div>
</div>


<style>
    /* Add your styles here */

    .bento {
        display:flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin: auto;
    }

    .container {
        margin: 0 auto;
        padding: 20px;
    }

    .header {
        text-align: center;
        margin-bottom: 40px;
    }

    .header h1 {
        font-size: 36px;
        color: #333;
        margin: 0;
        padding: 0;
    }

    .product-list {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 40px;
    }

    .product-card {
        height: 200px;
        width: 200px;
        background-color: #712;
        border-radius: 8px;
        padding: 20px;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }

    .product-card img {
        width: 100%;
        max-height: 200px;
        object-fit: cover;
        border-radius: 8px;
        margin-bottom: 10px;
    }

    .product-card h2 {
        font-size: 18px;
        color: #333;
        margin: 0;
        padding: 0;
        margin-bottom: 10px;
    }

    .text {
        text-align: center;
        margin-bottom: 40px;
    }
</style>