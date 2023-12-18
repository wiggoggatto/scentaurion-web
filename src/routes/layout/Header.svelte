<script>
	export let title = "Scentaurion";
	// export let subtitle = "Tailor-made Scents";

	let features = [
		"Unique Fragrances",
		"Personalized Blends",
		"Long-lasting Scents",
	];

	let isSmallScreen = false;

	function toggleMenu() {
		isSmallScreen = !isSmallScreen;
	}
</script>


<div class="header">
    <div class="flat left">
	    <img src="path/to/your/logo.png" alt="Scentaurion Logo" />
	    <a href="/"><h1>{title}</h1></a>
	    <!-- <h2>{subtitle}</h2> -->
    </div>
    
    <div class="flat">
	    <ul>
	    	<li>Catalogue</li>
            <li>Customize</li>
            <li>Order</li>
            <li>FAQ</li>
	    </ul>
    </div>

    <div class="flat right">
        <ul>
        	<a href=/login><li>Log In</li></a>
            <a href=/signup><li>Sign Up</li></a>
        </ul>
    </div>

	<div on:click={toggleMenu} class="burger-menu">
		☰
	</div>
</div>

<style>
	/* Add your custom styles here */
	.header {
		display: flex;
		flex-direction: row;
        justify-content: space-between;
        content-align: center;
        background-color: red;
        width: 100%;
	}

	img {
		max-width: 50px;
		max-height: 50px;
	}

	h1 {
		margin: 5px 0;
		font-size: 1.5em;
	}

	h2 {
		margin: 0;
		font-size: 1.2em;
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

    .right {
        align-items: flex-end;
        right: 0;
    }

    .left {
        left:0;
        align-items: flex-start;
    }

	@media only screen and (max-width: 600px) {
		.burger-menu {
			display: block;
		}

		ul {
			display: none;
		}

		.burger-menu.active + ul {
			display: flex;
		}
	}
</style>

