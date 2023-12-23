<script>
    import Header from '../layout/Header.svelte';
    import Footer from '../layout/Footer.svelte';

    let isSigned = false;
</script>

<Header />

<div>
    <div>
        <h1>Fragrance Profiles</h1>
        <p> INSERT DESCRIPTION HERE </p>
        <a href='/wiki/oil_based_perfume'>
            <p>Top notes →</p>
        </a>
        <a href='/wiki/water_based_perfume'>
            <p>Heart notes →</p>
        </a>
        <a href='/wiki/other_mediums'>
            <p>Base notes →</p>
        </a>
    </div>

    <div>
        <h1>Scent Families</h1>
        <p>Fragrances are categorized based on the scents they produce. Each scent is unique and significant- having their own characteristics, strengths and weaknesses.</p>
        <a href='/wiki/woody'>
            <p>Woody Scents →</p>
        </a>
        <a href='/wiki/citrus'>
            <p>Citrus Scents →</p>
        </a>
        <a href='/wiki/floral'>
            <p>Floral Scents →</p>
        </a>
        <a href='/wiki/fruity'>
            <p>Fruity Scents →</p>
        </a>
        <a href='/wiki/spicy'>
            <p>Spicy Scents →</p>
        </a>
        <a href='/wiki/fresh'>
            <p>Citrus Scents →</p>
        </a>
        <a href='/wiki/aquatic'>
            <p>Citrus Scents →</p>
        </a>
        <a href='/wiki/gourmand'>
            <p>Citrus Scents →</p>
        </a>
        <a href='/wiki/other'>
            <p>Other ingredients →</p>
        </a>
    </div>

    <div>
        <h1>Types of Perfume</h1>
        <p>Just as essential as the notes themselves, the way it's expressed impacts to the final symphony of the fragrance.</p>
        <a href='/wiki/oil_based_perfume'>
            <p>Oil-Based Perfume→</p>
        </a>
        <a href='/wiki/water_based_perfume'>
            <p>Alcohol-Based Perfume →</p>
        </a>
        <a href='/wiki/other_mediums'>
            <p>Other Mediums →</p>
        </a>
    </div>

    <div>
        <h1>Occasion, Season and Utility</h1>
        <p>Insert description here. </p>
        <a href='/wiki/climates'>
            <p>Different Climates Affecting Fragrances →</p>
        </a>
        <a href='/wiki/season'>
            <p>Changing Seasons Affecting Fragrances →</p>
        </a>
        <a href='/wiki/occasion'>
            <p>Best Perfume According to Events →</p>
        </a>
    </div>
</div>
<Footer />