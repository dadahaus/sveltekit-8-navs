<script>
	// import '../app.postcss';
	// import Header from './Header.svelte';
	import '../scss/style.css'
	import Nav from './components/Nav.svelte';

</script>

<div class="app">
	<Nav />

	<main>
		<slot />
	</main>

	<footer>
		<h1>this is the footer</h1>
	</footer>
</div>

<style lang="scss">

</style>
