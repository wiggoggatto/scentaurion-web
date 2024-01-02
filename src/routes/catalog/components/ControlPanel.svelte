<!-- src/components/ControlPanel.svelte -->

<script>
	// Add necessary logic for controlling ratings and types
</script>

<div class="control-panel">
	<!-- Add controls for ratings and types here -->
	<div>
		<label>Ratings:</label>
		<select>
			<option value="1">1⭐</option>
			<option value="2">2⭐</option>
			<option value="3">3⭐</option>
			<option value="4">4⭐</option>
			<option value="5">5⭐</option>
		</select>
	</div>
	<div>
		<label>Product Types:</label>
		<select>
			<option value="perfume">Perfume</option>
			<option value="hair_care">Hair Care</option>
		</select>
	</div>
	<div>
		<label>Scent Family:</label>
		<select>
			<option value="floral">Floral</option>
			<option value="citrus">Citrus</option>
		</select>
	</div>
</div>

<style>
	select {
		margin: 1em;
	}
	.control-panel {
		display: flex;
		flex-direction: row;
	}
</style>
