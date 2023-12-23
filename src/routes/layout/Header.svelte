<script>
	export let title = "Scentaurion.";
    let Search = new URL('./images/search.png', import.meta.url).href
    let Location = new URL('./images/location.png', import.meta.url).href
    let Cart = new URL('./images/cart.png', import.meta.url).href
    let Account = new URL('./images/account.png', import.meta.url).href
</script>


<div class="header">
	<!-- show the desktop version if in desktop, else show the small screen version. -->
    <div class="top">
		<div class=name>
			<a href="/" class="title"><h1>{title}</h1></a>
		</div>
    </div>
    <div class="bottom">
		<ul>
			<a href=/collections class="subtags"><li>COLLECTIONS</li></a>
			<a href=/catalog class="subtags"><li>CATALOG</li></a>
			<a href=/customize class="subtags"><li>CUSTOMIZE</li></a>
			<!-- <a href=/login><li>Log In</li></a> -->
		</ul>
	</div>	
	<div class="floating right">
		
		<a href="/location" class="floating-text">
			<img src={Location} alt="Location of our businesses."/>
		</a>

		<a href="/cart" class="floating-text">
			<img src={Cart} alt="Your shopping cart."/>
		</a>

		<a href="/login" class="floating-text">
			<img src={Account} alt="Login page."/>
		</a>
	</div>
	
	<div class="floating left">
		<a href="/search" class="floating-text">
			<img src={Search} alt="Search"/>
		</a>
	</div>

	<!-- <div class="burger-menu" on:click={toggleMenu}>
		<svg width="24" height="24" viewBox="0 0 24 24">
			<path fill="#fff" d="M0 0h24v24H0z" fill-opacity="0.0"/>
			<path fill="#fff" d="M3 18h18v-2H3v2zM3 6v2h18V6H3zm0 7h18v-2H3v2z"/>
		</svg>
	</div> -->
</div>

<style>
	/* Add your custom styles here */
	
	.header {
		display: flex;
		flex-direction: column;
        content-align: center;
        background-color: #111111;
		padding:auto;
		margin: 0;
        width: 100%;
	}

	.top {
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
		padding: 0 16px;
		background-color: #111111;
		color: #fff;
	}

	.bottom {
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
		padding: 0 16px;
		background-color: #111111;
		color: #fff;
	}

	img {
		max-width: 50px;
		max-height: 50px;
	}

	h1 {
		margin: 8px;
		font-size: 2em;
	}

	.title {
		margin: 0;
		color: #fff;
		text-decoration: none;
		font-family:'Kalnia', serif;
		font-size: 1.5em;
	}

	.title:hover {
		color: #7c5295;
	}

	.subtags {
		margin: 0 16px;
		color: #fff;
		text-decoration: none;
		font-family: 'Playfair', serif;
		font-size: 1em;
	}

	.floating {
		position: absolute; /* Added absolute positioning */
    	display: flex;
    	justify-content: flex-end;
    	align-items: center;
    	gap: 16px;
	}

	.right {
		top: 1em;
		right: 1em;
	}

	.left {
		top: 1em;
		left: 1em;
	}

	.label-location {
		display: none;
	}

	.location:hover + .label-location {
		display: block;
		color: #663a82;
	}



	.subtags:hover {
		color: #663a82;
	}

	ul {
		list-style-type: none;
		padding: 0;
		margin: 10px 0;
		display: flex;
		flex-direction: row;
		justify-content: flex-start;
		align-items: flex-start;
	}

	li {
		margin-bottom: 5px;
	}

	.burger-menu {
		display: none;
		cursor: pointer;
	}

    .flat {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

	@media only screen and (max-width: 600px) {
		.top {
			display: flex;
			flex-direction: row;
			align-items: flex-start;
			padding: 0 16px;
			background-color: #111111;
			color: #fff;
		}

		.name {
		}

		.burger-menu {
			display: block;
		}

		ul {
			display: none;
		}

		.burger-menu.active + ul {
			display: flex;
		}

		.floating {
        	display: none;
    	}
	}


	.material-symbols-outlined {
		font-variation-settings:
		'FILL' 0,
		'wght' 400,
		'GRAD' 0,
		'opsz' 24
	}

</style>

