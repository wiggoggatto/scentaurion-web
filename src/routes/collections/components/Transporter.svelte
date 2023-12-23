<script>
    let boxItems = [
        { id: 1, bind: '/', series: 'GIRLBOSS' },
        { id: 2, bind: '/', series: 'FAIRYTALE' },
        { id: 3, bind: '/', series: 'UNMELTING' },
    ];

    function handleClick(item) {
        console.log(`Clicked on item with id ${item.id}`);
    }
</script>

<style>
    .box {
        display: flex;
        flex-direction:row;
        justify-content: center;
        height: 3em;
        padding: 10px;
        background-color: #ECEEEC;
    }

    .box-item {
        align-self: center;
        border: 1px solid black;
        margin: 6px;
        cursor: pointer;
    }

    .box-item:hover {
        background-color: gray;
    }

    .box-item a {
        text-decoration: none;
    }

    .box-item p {
        margin: 2px;
        padding: 6px;
    }
</style>

<div class="box">
    {#each boxItems as item (item.id)}
        <div class="box-item" on:click={() => handleClick(item)}>
            <a href={item.bind}> 
                <p>{item.series}</p>
            </a>
        </div>
    {/each}
</div>
