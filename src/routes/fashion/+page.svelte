<script>
    import one from '$lib/fashion/fashion-1.jpeg'; 
    import two from '$lib/fashion/fashion-2.jpeg'; 
    import three from '$lib/fashion/fashion-3.jpeg'; 
    import four from '$lib/fashion/fashion-4.jpeg'; 
    import five from '$lib/fashion/fashion-5.jpeg'; 
    import six from '$lib/fashion/fashion-6.jpeg'; 
    import seven from '$lib/fashion/fashion-7.jpg'; 
    import eight from '$lib/fashion/fashion-8.jpg'; 
    import nine from '$lib/fashion/fashion-9.jpg'; 
    import ten from '$lib/fashion/fashion-10.jpg'; 
    import eleven from '$lib/fashion/fashion-11.jpg'; 
    import twelve from '$lib/fashion/fashion-12.jpg'; 
    import thirteen from '$lib/fashion/fashion-13.jpg'; 
    import fourteen from '$lib/fashion/fashion-14.jpg'; 
    import fifteen from '$lib/fashion/fashion-15.jpg'; 
    import sixteen from '$lib/fashion/fashion-16.jpg'; 
    import seventeen from '$lib/fashion/fashion-17.jpg'; 
    import eighteen from '$lib/fashion/fashion-18.jpg'; 
    import nineteen from '$lib/fashion/fashion-19.jpg'; 
    import twenty from '$lib/fashion/fashion-20.jpg'; 
    import twentyOne from '$lib/fashion/fashion-21.jpg'; 
    import twentyTwo from '$lib/fashion/fashion-22.jpg'; 
    import twentyThree from '$lib/fashion/fashion-23.jpg'; 
    import twentyFour from '$lib/fashion/fashion-24.jpg'; 


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
        fourteen,
        fifteen, 
        sixteen, 
        seventeen, 
        eighteen, 
        nineteen, 
        twenty, 
        twentyOne, 
        twentyTwo, 
        twentyThree, 
        twentyFour
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
            <a href="/food">Food</a>
        </div>

        <div class="lg"></div>

    </div>
</div>
