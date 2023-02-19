<script>
<<<<<<< HEAD
	// import '../app.postcss';
	// import Header from './Header.svelte';
	import '../scss/style.css'
	import Nav from './components/Nav.svelte';

</script>

<div class="app">
	<Nav />
=======
	// import { COLOR } from './../../.svelte-kit/ambient.d.ts';
	// import '../app.postcss';

	// import './styles.css';
	import '../scss/style.css';
	import Footer from './components/Footer.svelte';
	import List from './components/List.svelte';
</script>

<div class="app">
>>>>>>> 3463c2a4597ac5cf8a02b438428273865e218084

<List/>
	<main>
		<slot />
	</main>

	
	<Footer>
		<slot />
	</Footer>
</div>

<<<<<<< HEAD
<style lang="scss">

=======
<style>
a{
	color: inherit;

}
>>>>>>> 3463c2a4597ac5cf8a02b438428273865e218084
</style>
