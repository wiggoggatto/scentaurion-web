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
        cost: '115.00',
        label: 'HAIR CARE PRODUCT',
        description: 'Composed of notes of bergamot, lemon, and orange, this fragrance is a citrusy delight.',
      },
      {
        id: 2,
        title: 'Product 2',
        cost: '$50.00',
        label: 'OIL-BASED PERFUME',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
      },
      {
        id: 3,
        title: 'Product 2',
        cost: '$50.00',
        label: 'New',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
      },
      {
        id: 4,
        title: 'Product 2',
        cost: '$50.00',
        label: 'New',
        description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
      },      
      // Add more product entries as needed
    ];
</script>

<Header/>

    <div class="center">
        <!-- add conditional render where it renders control panel wide when in desktop and control panel small when in mobile -->
        <div class="control-panel-wide">
            <h2>Premium Fragrances at Scentaurion</h2>
            <ControlPanel />
        </div>
        <div class="product-list">
            <ProductList {products} />
        </div>
    </div>
<Footer/>

<style>
    main {
        display: flex;
        flex-direction: column;
    }

    .center {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

    .product-list {
        /* background-color: #456; */
		flex: 1; 
		display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        width: 80%;
		/* flex-wrap: wrap; */
	}

    .control-panel-wide {
        text-align: center;
        align-items: center;
        justify-content: center;
    }
</style>

