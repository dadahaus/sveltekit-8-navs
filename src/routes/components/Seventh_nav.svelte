<script>
	import { page } from '$app/stores';
</script>

<nav>
	<ul>
		<div class="right_nav">
			<a href="http://"><li>work</li></a>
			<a href="http://"><li>about</li></a>
			<a href="http://"><li>contact</li></a>
			<a href="/"> <img src="src/assets/dribbble.svg" alt="logo" srcset="" /> </a>
		</div>
	</ul>
</nav>

<style lang="scss">
	nav {
		padding: 1rem 2rem 1rem 2rem;
		position: fixed;
		width: 100%;
		top: 0;
		text-transform: uppercase;
		font-weight: 700;
		ul {
			display: flex;
			align-items: center;
			justify-content: space-between;
			gap: 5rem;

			.right_nav {
				display: flex;
				align-items: center;
				justify-content: flex-end;
				flex: 1;
				gap: 2rem;
				img {
					width: 4rem;
					height: 4rem;
				}
			}
		}
	}
</style>
