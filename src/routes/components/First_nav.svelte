<script>
	// import { page } from '$app/stores';
</script>

<nav class="first_nav">
	<ul>
		<div class="left_nav"><a href="">MENU</a></div>
		<div class="center_nav"><a href="">WORK</a></div>
		<div class="right_nav"><a href="">US</a></div>
	</ul>
</nav>

<style lang="scss">
	.first_nav {
		padding: 2rem;
		position: fixed;
		width: 100%;
		top: 0rem;
		a {
			text-decoration: none;
			color: inherit;
			font-size: 1.2rem;
		}
		ul {
			display: flex;
			align-items: center;
			justify-content: space-between;
			gap: 5rem;
			text-transform: uppercase;
			& > * {
				display: flex;
				justify-content: center;
			}
			.left_nav {
				flex: auto;
			}
			.center_nav {
				flex: auto;
			}
			.right_nav {
				flex: auto;
			}
		}
	}
</style>
