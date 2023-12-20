<script>
	export let products;
</script>

<div class="product-list">
	{#each products as product (product.id)}
		<div class="product-item">
			<img src={product.image} alt={product.title} />
			<h3>{product.title}</h3>
			<p>{product.cost}</p>
			<span class="label">{product.label}</span>
			<p>{product.description}</p>
		</div>
	{/each}
</div>

<style>
    .product-list {
        display:flex;
        flex-direction:row;
    }

	.product-item {
		width: 200px; /* Set a specific width for each product item */
		margin: 16px;
		padding: 16px;
        border-radius: 12px;
		border: 1px solid #ddd; /* Add a border for better visibility */
	}

	.product-details {
		margin-top: 8px;
	}
</style>
