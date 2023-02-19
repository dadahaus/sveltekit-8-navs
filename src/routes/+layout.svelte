<script>
	// import { COLOR } from './../../.svelte-kit/ambient.d.ts';
	// import '../app.postcss';

	// import './styles.css';
	import '../scss/style.css';
	import Footer from './components/Footer.svelte';
	import List from './components/List.svelte';
	import Nav from './components/Nav.svelte';
</script>

<div class="app">
	<Nav />
	<main>
		<slot />
	</main>
	<List />

	<Footer>
		<slot />
	</Footer>
</div>

<style lang="scss">
</style>
