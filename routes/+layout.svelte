<script>

    import Navbar from './navbar.svelte'; 
    import Footer from './footer.svelte'; 

    export let data;
    import { fly, fade, slide, scale } from 'svelte/transition';
	import { afterNavigate, disableScrollHandling } from '$app/navigation';

    //this fixes the snap to the top on page transition. 
	afterNavigate(() => {
    	disableScrollHandling();
    	setTimeout(() => {
        scrollTo({ top: 0, behavior: 'instant' });
    	}, 300);
	});

</script>

<style>
    @import url(style.css);
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,500;0,600;0,700;0,800;0,900;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
</style>


{#key data.pathname}
<Navbar />
	<div in:fly={{y:10, duration: 200, delay: 300 }} out:fly={{y:-10, duration: 200 }}>
		<slot />
<Footer /> 
	</div>
{/key}