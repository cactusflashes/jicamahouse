<script>
    import one from '$lib/food/food-1.jpg'; 
    import two from '$lib/food/food-2.jpg'; 
    import three from '$lib/food/food-3.jpg'; 
    import four from '$lib/food/food-4.jpg'; 
    import five from '$lib/food/food-5.jpg'; 
    import six from '$lib/food/food-6.jpg'; 
    import seven from '$lib/food/food-7.jpg'; 
    import eight from '$lib/food/food-8.jpg'; 
    import nine from '$lib/food/food-9.jpg'; 
    import ten from '$lib/food/food-10.png'; 
    import eleven from '$lib/food/food-11.png'; 
    import twelve from '$lib/food/food-12.png'; 

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
        twelve
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
            <a href="/product">Product</a>
            <a href="/fashion">Fashion</a>
        </div>

        <div class="lg"></div>


    </div>
</div>
