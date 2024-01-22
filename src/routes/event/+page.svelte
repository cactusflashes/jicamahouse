<script>
    import one from '$lib/event/event-1.jpg'; 
    import two from '$lib/event/event-3.jpg'; 
    import three from '$lib/event/event-4.jpg'; 
    import four from '$lib/event/event-2.jpg'; 
    import five from '$lib/event/event-5.jpeg'; 
    import six from '$lib/event/event-6.jpeg'; 
    import seven from '$lib/event/event-7.jpg'; 
    import eight from '$lib/event/event-10.jpg'; 
    import nine from '$lib/event/event-9.jpg'; 
    import ten from '$lib/event/event-8.jpg'; 
    import eleven from '$lib/event/event-11.jpg'; 
    import twelve from '$lib/event/event-12.jpg'; 
    import thirteen from '$lib/event/event-13.jpeg'; 
    import fourteen from '$lib/event/event-14.jpeg'; 
    import fifteen from '$lib/event/event-15.jpg'; 
    import sixteen from '$lib/event/event-16.jpg'; 
    import seventeen from '$lib/event/event-17.jpg'; 
    import eighteen from '$lib/event/event-18.jpg'; 
    import nineteen from '$lib/event/event-19.jpeg'; 
    import twenty from '$lib/event/event-20.jpeg'; 
    import twentyOne from '$lib/event/event-21.png'; 
    import twentyTwo from '$lib/event/event-22.png'; 
    import twentyThree from '$lib/event/event-23.jpg'; 
    import twentyFour from '$lib/event/event-24.jpg'; 

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
            <a href="/fashion">Fashion</a>
            <a href="/product">Product</a>
            <a href="/food">Food</a>
        </div>

        <div class="lg"></div>


    </div>
</div>
