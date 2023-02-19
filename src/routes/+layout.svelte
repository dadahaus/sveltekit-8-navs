<script>
	// import { COLOR } from './../../.svelte-kit/ambient.d.ts';
	// import '../app.postcss';

	// import './styles.css';
	import '../scss/style.css';
	import Footer from './components/Footer.svelte';
	import List from './components/List.svelte';
</script>

<div class="app">

<List/>
	<main>
		<slot />
	</main>

	
	<Footer>
		<slot />
	</Footer>
</div>

<style>
a{
	color: inherit;

}
</style>
