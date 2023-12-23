<script>
    import Header from '../layout/Header.svelte';
    import Footer from '../layout/Footer.svelte';
    import ProductList from './components/ProductList.svelte';
    import ControlPanel from './components/ControlPanel.svelte';

    // Sample product data
    let products = [
      {
        id: 1,
        title: 'Sophronia',
        image: 'path/to/image1.jpg',
        cost: '99.00',
        label: 'CLASSIC',
        description: 'Composed of notes of bergamot, lemon, and orange, this fragrance is a citrusy delight.',
      },
      {
        id: 2,
        title: 'Product 2',
        image: 'path/to/image1.jpg',
        cost: '$50.00',
        label: 'New',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
      },
      // Add more product entries as needed
    ];
</script>

<Header/>
    <br>
    <br>
    <main>
        <!-- add conditional render where it renders control panel wide when in desktop and control panel small when in mobile -->
        <div class="control-panel-wide">
            <ControlPanel />
        </div>
        <div class="product-list">
            <h2>Featured Fragrances </h2>
            <ProductList {products} />
        </div>
    </main>

    <br>
    <br>
<Footer/>

<style>
    main {
        display: flex;
    }

    .product-list {
        /* background-color: #456; */
		flex: 1; 
		display: flex;
        flex-direction: column;
		/* flex-wrap: wrap; */
	}

    .control-panel-wide {
        /* background-color: #987; */
        position: sticky;
		top: 0;
		align-self: flex-start; 
		margin-right: auto; 
		padding: 16px;
		/* box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); */
    }
</style>

