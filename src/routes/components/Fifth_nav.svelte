<script>
	import { page } from '$app/stores';
</script>

<h1>hi hi</h1>
<nav>
	<ul>
		<a href="http://" class="left_nav"> menu </a>
		<a href="http://" class="center_nav"> work </a>
		<a href="http://" class="right_nav"> us </a>
	</ul>
</nav>

<style lang="scss">
	nav {
		padding: 2rem 5rem 2rem 5rem;
		position: fixed;
		width: 100%;
		top: 0;
		text-transform: uppercase;
		font-weight: 700;
		display: flex;
		justify-content: center;
		ul {
			display: flex;
			align-items: center;
			& > * {
				padding: 0.5rem 1rem 0.5rem 1rem;
				border: solid white 0.1rem;
				color: white;
				min-width: 8ch;
				display: grid;
				place-content: center;
			}
			.left_nav {
				border-right: none;
				border-radius: 1rem 0 0 1rem;
			}
			.center_nav {
			}
			.right_nav {
				border-left: none;
				border-radius: 0 1rem 1rem 0;
			}
		}
	}
</style>
