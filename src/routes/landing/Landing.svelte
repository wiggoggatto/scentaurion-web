
<script>
    import BentoBox from "./components/BentoBox.svelte"
</script>

<div class="container">
    <div class="supercontainer">
        <div class="header">
            <div class="launch">
                <h1>Join Our Brand Launch</h1>
                <p>MSU-GSC Siklab at January 25 10AM-5PM</p>
                <p>Barangay Fatima, General Santos City 9500</p>
            </div>
            <div class="youtube">
                <iframe width="560" height="315" src="https://www.youtube.com/embed/AGCL3icu9dk?si=ZcoM3OIfBTDqxaUw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            </div>
        </div>
    </div>

    <div class="text">
        <h2>Latest in Scentaurion's Collection</h2>
        <div class="divide">
            <p>Girl Math Series</p>
        </div>
    </div>

    <div class="product-list">
        <div class="product-card design rose">
            <h2>Sophrania</h2>
            <div class="bg-blur">
                <p>Hair care oil with fragrance inspired by flowers found in Malacanang Palace.</p>
            </div>
        </div>
        <div class="product-card design sunflower">
            <h2>Aethlyn</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </div>
        <div class="product-card design lavander">
            <h2>Perfume 3</h2>
            <p>Lorem ipsum dolor sit amet, consecstetur adipiscing elit.</p>
        </div>
    </div>

    <div class="bento">
        <BentoBox/>
    </div>

    <div class="text">
        <a href="/customize">
            <h2>Craft Your Signature Scent</h2>
        </a>
        <div class="divide">
            <p>Learn, create, and personalize your own fragrance masterpiece.</p>
        </div>
    </div>

    <div class="text">
        <a href="/">
            <h2>Changing Society One Scent at A Time</h2>
        </a>
            <p>For every purchase, we donate a portion of the proceeds to a charity.</p>
    </div>

    <div class="text">
        <h2>Sustainability and Ethical Production</h2>
        <p>ADJECTIVE how our strict ethical production protocols.</p>
    </div>    

    
</div>


<style>
    /* Add your styles here */
    

    .bento {
        display:flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 100%;
        padding-top: 3em;
        padding-bottom: 3em;
        background-color: #e9e1f7;
    }

    .supercontainer {
        width: 100%;
    }
    
    .container {
        display: flex;
        flex-direction: column;
        width: 100%;
        max-width: 100%; /* Ensure it doesn't exceed the viewport width */
        margin: 0; /* Center the container horizontally */
    }

    .divide{
        display: flex;
        align-items: center;
    }

    .divide::before, .divide::after {
        flex: 1;
        content: '';
        padding:0.4px;
        background-color: #667;
        margin:5px;
    }

    .design {
        background-size: cover;
        width: 100%;
    }

    .rose {
        background-image: url("./images/roses.jpg");
    }

    .sunflower {
        background-image: url("./images/sunflower.jpg");
    }

    .lavander {
        background-image: url("./images/lavander.jpg");
    }

    .header {
        background-image: url("./images/bg_img3.png");
        background-size: cover;
        width: 100%;
        height: 35em;
        display:flex;
        flex-direction: row;
    }

    .header h1 {
        font-size: 3em;
        color: #F5F5DC;
    }

    .header p {
        font-size: 1.2em;
        color: #F5F5D2;
    }

    .launch {    
        margin-top: 10em;
        margin-left: 4em;
    }

    .youtube {
        margin-top: 8em;
        margin-left: 10em;
    }

    .product-list {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        margin-top: 3em;
        margin-bottom: 5em;
        gap: 3em;
    }

    .product-card {
        height: 12em;
        width: 10em;
        /* background-color: rgba(0, 0, 0, 0.1); */
        border-radius: 10px;
        padding: 20px;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
    }

    .product-card img {
        width: 100%;
        max-height: 200px;
        object-fit: cover;
        border-radius: 8px;
        margin-bottom: 10px;
    }

    .product-card h2 {
        font-size: 20px;
        color: #fafafa;
        margin-top: 1em;
        padding: 0;
        margin-bottom: 10px;
    }

    .product-card p {
        font-size: 18px;
        color: #F5F5D2;
    }

    .text {
        text-align: center;
        margin-top: 4em;
    }

    .text a {
        text-decoration: none;
        color: #010101;
    }

    .text a:hover {
        color: red;
    }

    .text h2 {
        font-size: 2em;
    }

    .text p {
        font-size: 1.2em;
        /* margin-bottom: 3em; */
    }
    
    @media only screen and (max-width: 600px) {
        .header {
            background-image: url("./images/bg_img3.png");
            background-size: cover;
            width: 100%;
            height: 45em;
            display:flex;
            flex-direction: column;
        }

        .launch {    
            margin-top: 4em;
            margin-left: 4em;
        }

        .youtube {
            justify-content: center;
            align-items: center;
            margin: 1em;
        }

        .youtube iframe {
            width: 100%;
            height: 100%;
        }
    }
</style>