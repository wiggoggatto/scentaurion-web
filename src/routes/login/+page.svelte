
<script>
    import Header from '../layout/Header.svelte';
    import Footer from '../layout/Footer.svelte';
</script>

<Header/>

<div class="main">
    
    <h1>Login to Account</h1>
    <div class="options">
        <div>
            <h2>Username</h2>
            <input>
            <h2>Password</h2>
            <input>
        </div>
    

        <div class="providerLogin">
            <button>Login with Google</button>
            <button>Login with Apple</button>
            <button>Login with Facebook</button>
            <button>Login with Twitter</button>
        </div>
    </div>
    <h3>Have no account? <a href="/signup">Sign up instead</a></h3>
</div>

<Footer/>


<style>
    .main {
        display:flex;
        flex-direction:column;
        justify-content: center;
        align-items: center;
    }

    /* have media query so that the option flex becomes column when on small screens */
    .options {
        display:flex;
        flex-direction: row;
    } 


    .providerLogin {
        display:flex;
        flex-direction:column;
    }
</style>
