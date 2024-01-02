<script>
	export let products;
</script>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<div class="product-list">
	{#each products as product (product.id)}
		<div class="product-item">
			<h3>{product.title}</h3>
			<!-- <img src={product.image} alt={product.title} /> -->
			<p>{product.cost}</p>
			<p>{product.description}</p>
			<span class="label">{product.label}</span>
		</div>
	{/each}
</div>

<style>
    .product-list {
        display:flex;
        flex-direction: row;
		flex-wrap: wrap;
		width: 100%;
    }

	.checked {
  		color: orange;
	}	

	.product-item {
		display: flex;
		flex-direction: column;
		width: 180px; /* Set a specific width for each product item */
		height: 260px;
		margin: 1.2em;
		padding: 16px;
        border-radius: 12px;
		border: 1px solid #ddd; /* Add a border for better visibility */
	}

	.product-details {
		margin-top: 8px;
	}

	.label {
		align-items: flex-end;
		background-color: red;
	}
</style>
