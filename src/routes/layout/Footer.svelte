<script>
    let Logo = new URL('./images/logo.png', import.meta.url).href
</script>


<div class="info">
    <div class="upper">
        <div class="logo">
            <img src={Logo} alt="Scentaurion's Logo"/>
        </div>

        <div class="box">
            <h3>Contact Us</h3>
            <p>Towerjen Suites, Dacera Avenue</p>
            <p>City Heights, General Santos City 9500</p>
            <p>corporate.scentaurion@gmail.com</p>
            <p>DITO +63 994 461 1776 </p>
        </div>
        <div class="box">
            <h3>About Us</h3>
            <p>Our Mission</p>
            <p>Our Impact</p>
            <p>The History</p>
            <p>The Executives</p>
        </div>
    </div>
    
    <footer>
        <p>&copy; 2024 Ravin Chavez. All rights reserved.</p>
    </footer>
</div>


<style>
    .info {
        display: flex;
        flex-direction: column;
        background-color:  #111111;
        color: white;
        padding: 20px;
    }

    footer {
        display: flex;
        justify-content: center;
        align-items: center;
        background-color:  #111111;
    }

    .upper {
        display: flex;
        flex-direction: row;
    }

    .box {
        display:flex;
        flex-direction:column
    }

    .box p {
        margin:2px;
    }

    .logo {
        margin: 0 20px;
    }

    .logo img {
        width: 100px;
        height: 100px;
    }
</style>