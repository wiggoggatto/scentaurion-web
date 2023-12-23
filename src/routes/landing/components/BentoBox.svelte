<script>
</script>
   
<div class="text">
    <h2><a href="/customize">Discover Your Signature Scent</a></h2>
    <div>
        <p>
            Find out what scents are best for you and your loved ones.
        </p>
    </div>
</div>
<div class="center-pls">
<div class="main-compsce">
    <div class="topic">
        <h4>Environment.</h4>
        <p>Search the factors that affect how your fragrance works.</p>
    </div>
    <div class="topic">
        <h4>Lifestyle.</h4>
        <p>Lifestyle can reveal the optimum way to indulge in your perfume.</p>
    </div>                
    <div class="topic">
        <h4>Preferences.</h4>
        <p>Find the scents that you prefer.</p>
    </div>
    <div class="topic">
        <h4>Projection.</h4>
        <p>Peek into your inner and outside worlds.</p>
    </div>   
    <div class="topic">
        <h4>History.</h4>
        <p>The products you patronize in the past might reveal something about you...</p>
    </div>
    <div class="topic">
        <h4>Sensitivity.</h4>
        <p>The fragrances that you dislike or are allergic to.</p>
    </div>
</div>
</div>

<style>
    .text {
        grid-column: 1 / span 3;
        text-align: center;
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
    }

    .center-pls {
        display:flex;
        justify-content: center;
        align-items: center;
        margin-bottom: 3em;
    }
       

    .main-compsce {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        grid-gap: 10px;
    }

    .topic {
        max-width: 200px;
        margin-top: 20px;
        padding-right: 10px;
    }


    .divide{
        display: flex;
        align-items: center;
    }

    .divide::before, .divide::after {
        flex: 1;
        content: '';
        padding:0.4px;
        background-color: #111;
        margin:5px;
    }
    

    .main-compsce h4, .main-compsce p {
        margin: 0;
    }
</style>
