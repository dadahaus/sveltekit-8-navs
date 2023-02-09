<script>
	import '../app.postcss';

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
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
		background-color: black;
		color: antiquewhite;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
