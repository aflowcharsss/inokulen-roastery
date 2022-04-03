<script context="module">
	export const prerender = true;
</script>

<script>
	import Hero from '../components/Hero.svelte';
	import Feature from '../components/Feature.svelte';
	import Catalog from '../components/Catalog.svelte';
	import Testimony from '../components/Testimony.svelte';
	import Subscribe from '../components/Subscribe.svelte';
</script>

<svelte:head>
	<title>Rumah &minus; Inokulen Roastery</title>
</svelte:head>

<section class="hero">
	<Hero />
</section>
<section class="feature">
	<Feature />
</section>
<section class="catalog">
	<Catalog />
</section>
<section class="testimony">
	<Testimony />
</section>

<section class="subscribe">
	<Subscribe />
</section>

<style>
	section.hero {
		@apply py-8;
	}

	section {
		@apply py-16;
	}

	section.subscribe {
		@apply mt-8;
	}
</style>
