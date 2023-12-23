<script>
    import Header from '../layout/Header.svelte';
    import Footer from '../layout/Footer.svelte';
    import Transporter from './components/Transporter.svelte';
</script>

<Header />

<div>
    <div class="landing start">
        <h1>Our Coveted Collections</h1>
        <Transporter />
    </div>

    <div class="semi-landing sections">
    </div>

    <div class="scheme clt-girlboss sections">
        <div class="meat">            
            <h3>THE GIRLBOSS SERIES</h3>
            <p>COMPOSED WITH X, Y, Z NOTES</p>
            <!-- <p>She was a fairy, a wild sprite, a pixie.</p> DESCRIPTION OF EACH PERFUME -->
        </div>
        <div class="image">
            IMAGE HERE
        </div>
    </div>

    <br>
    <br>

    <div class="clt-fairytale scheme">
        <div class="image">
            IMAGE HERE
        </div>
        <div class="meat">            
            <h3>THE GIRLBOSS SERIES</h3>
            <p>COMPOSED WITH X, Y, Z NOTES</p>
            <!-- <p>She was a fairy, a wild sprite, a pixie.</p> DESCRIPTION OF EACH PERFUME -->
        </div>
    </div>
</div>

<Footer />

<style>

.start {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.scheme {
    display:flex;
    flex-direction:row;
}

.landing {
    height: 36vh;
}

.landing h1 {
    font-size: 2rem;
    color: #111;
}

.landing p {
    font-size: 1rem;
    color: #222;
}

.clt-girlboss {
    width: 100vw;
}

.meat{
    display: flex;
    flex-direction: column;
    align-content: center;
    justify-content: center;
    width: 60vw;
}

.image{
    width: 40vw;
}

.clt-fairytale {
    width: 100vw;
}

.frt-oea{
    display: flex;
    flex-direction: column;
    align-content: center;
    justify-content: center;
    width: 60vw;
}

.frt-right{
    width: 40vw;
}
</style>
