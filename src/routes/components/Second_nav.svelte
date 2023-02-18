<script>
	import { page } from '$app/stores';
</script>

<nav class="second_nav">
	<ul>
		<div class="left_nav">
			<a href="/"> <img src="src/assets/dribbble.svg" alt="logo" srcset=""> </a>
	  
		  </div>

		<div class="right_nav">
			<a href="">services</a>
			<a href="">work</a>
			<a href="">about</a>
			<a href="">contact</a>
		</div>
	</ul>
</nav>

<style lang="scss">
	.second_nav {
		padding: 1rem 2rem 1rem 2rem;
		position: fixed;
		width:100%;
		top: 0;
		text-transform: uppercase;
		font-weight: 700;
		a {
			text-decoration: none;
			color: inherit;
			font-size: 1.2rem;
		}
		ul {
			display: flex;
			align-items: center;
			justify-content: space-between;
			// height: 3rem;
			gap: 5rem;
			.left_nav {
				flex: auto;
				img {
					width: 3rem;
					height: 3rem;
				}
			}
			.right_nav {
				display: flex;
				flex: auto;
				justify-content: flex-end;
				align-items: flex-end;
				height: 100%;
				gap: 1rem;
			
				img {
					width: 3rem;
					height: 3rem;
				}
			}
		}
	}
</style>
