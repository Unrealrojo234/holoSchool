<script>
	import History from './History.svelte';
	import Board from './Board.svelte';
	import Cards from './Cards.svelte';
	import Benefits from './Benefits.svelte';
	import Trial from './Trial.svelte';
	import Footer from './Footer.svelte';
	import Map from './Map.svelte';
	import Results from './Results.svelte';
	import Images from './Images.svelte';
</script>

<main class="container-fluid">
	<h1 class="text-center prosto-one-regular">Holo Secondary School</h1>
	<History />
	<Images />
	<Board />
	<Cards />
	<Benefits />
	<Results />
	<Map />
	<Footer />
	<Trial />
</main>

<style>
	.prosto-one-regular {
		font-family: 'Prosto One', sans-serif;
		font-weight: 800;
		font-style: normal;
	}

	h1 {
		font-size: 3.5rem;
	}
</style>
