<script>
    import one from '$lib/product/product-1.jpg'; 
    import two from '$lib/product/product-2.jpg'; 
    import three from '$lib/product/product-3.jpg'; 
    import four from '$lib/product/product-4.jpg'; 
    import five from '$lib/product/product-5.jpg'; 
    import six from '$lib/product/product-7.jpg'; 
    import seven from '$lib/product/product-8.jpg'; 
    import eight from '$lib/product/product-9.jpg'; 
    import nine from '$lib/product/product-10.jpg'; 
    import ten from '$lib/product/product-11.png'; 
    import eleven from '$lib/product/product-12.png'; 
    import twelve from '$lib/product/product-13.jpg'; 
    import thirteen from '$lib/product/product-14.jpg'; 
    import fourteen from '$lib/product/product-15.jpg'; 

    let photoUrls = [
        one, 
        two, 
        three, 
        four, 
        five, 
        six, 
        seven, 
        eight, 
        nine, 
        ten, 
        eleven, 
        twelve, 
        thirteen, 
        fourteen
    ]; 

</script>

<div class="body">
    <div class="container">
        <div class="transparency-failover"></div>
        <a class="exit" href="/">
            <p>x</p>
        </a>
        <div class="md"></div>

        {#each photoUrls as photoUrl, index}
            {#if index % 2 === 0}
                <div class="photo-column">
                    <img src={photoUrl} class="photo" alt="mm" />
                    {#if photoUrls[index + 1]}
                        <img src={photoUrls[index + 1]} class="photo" alt="mm" />
                    {/if}
                </div>
            {/if}
        {/each}

        <div class="lg"></div>

        <div class="hop-to">
            <a href="/event">Event</a>
            <a href="/fashion">Fashion</a>
            <a href="/food">Food</a>
        </div>

        <div class="lg"></div>

    </div>
</div>
