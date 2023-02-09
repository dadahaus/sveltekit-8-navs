<script>
	// import '../app.postcss';

	// import './styles.css';
	import '../dist/style.css';
	import Footer from './components/Footer.svelte';

</script>

<div class="app">

	<main>
		<slot />
	</main>
	
	<Footer>
		<slot />
	</Footer>
</div>

<style>
</style>
