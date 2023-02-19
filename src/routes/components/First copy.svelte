<script>
	import { page } from '$app/stores';
</script>

<nav>
	<ul>
		<div class="left_nav">
			<li><a href="http://">home</a></li>
		</div>
		<div class="right_nav">
			<li><a href="http://">there</a></li>
			<li><a href="http://">yup</a></li>
			<li><a href="http://">first</a></li>
		</div>
	</ul>
</nav>

<style lang="scss">
	nav {
		padding: 2rem 5rem 2rem 5rem;
		ul {
			display: flex;
			align-items: center;
			justify-content: space-between;
			gap: 5rem;
			text-transform: uppercase;
			.left_nav {
				flex-basis: 20%;
				img {
					width: 3rem;
					height: 3rem;
				}
			}
			.center_nav {
				flex: auto;
				display: flex;
				justify-content: space-evenly;
				text-transform: uppercase;
				font-weight: 900;
			}
			.right_nav {
				display: flex;
				justify-content: center;
				flex-basis: 30%;
				gap: 1rem;
				img {
					width: 3rem;
					height: 3rem;
				}
			}
		}
	}
</style>
