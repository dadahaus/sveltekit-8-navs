<script>
	import { page } from '$app/stores';
</script>

<nav>
	<ul>
		<div class="left_nav">
			<a href="/"> <img src="src/assets/dribbble.svg" alt="logo" srcset="" /> </a>
		</div>
		<div class="center_nav">
			<a href="http://"><li>menu</li></a>
			<a href="http://"><li>work</li></a>
			<a href="http://"><li>contact</li></a>
		</div>
		<div class="right_nav">
			<a href="http://"> <img src="src/assets/behance-2.svg" alt="logo" srcset="" /> </a>
			<a href="http://"><img src="src/assets/mail-1.svg" alt="logo" srcset="" /> </a>
			<a href="http://"><img src="src/assets/dribbble.svg" alt="logo" srcset="" /> </a>
		</div>
	</ul>
</nav>

<style lang="scss">
	nav {
		padding: 2rem;
		position: fixed;
		bottom: 0rem;
		width: 100%;
		text-transform: uppercase;
		ul {
			display: flex;
			align-items: center;
			justify-content: space-between;
			gap: 5rem;
			.left_nav {
				flex: 1;
				img {
					width: var(--nav-item);
					height: var(--nav-item);
				}
			}
			.center_nav {
				flex: 1;

				display: flex;
				justify-content: space-evenly;
				gap: 1rem;
				// text-transform: uppercase;
				font-weight: 900;
			}
			.right_nav {
				display: flex;
				justify-content: flex-end;
				gap: 1rem;
				flex: 1;
				// gap: 1rem;
				img {
					width: var(--nav-item);
					height: var(--nav-item);
				}
			}
		}
	}
</style>
