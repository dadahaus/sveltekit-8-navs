<script>
	import { page } from '$app/stores';
</script>

<nav class="third_nav">
	<ul>
		<div class="left_nav">
			<a href="/"> <img src="src/assets/dribbble.svg" alt="logo" srcset="" /> </a>
		</div>
		<div class="center_nav">
			<a href="/">see work</a>
		</div>

		<div class="right_nav">
			<input type="checkbox" id="nav__checkbox" class="nav__checkbox" />
			<label for="nav__checkbox" class="nav__toggle">
				<svg class="menu" viewBox="0 0 448 512" width="100" title="bars">
					<path
						d="M16 132h416c8.837 0 16-7.163 16-16V76c0-8.837-7.163-16-16-16H16C7.163 60 0 67.163 0 76v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16zm0 160h416c8.837 0 16-7.163 16-16v-40c0-8.837-7.163-16-16-16H16c-8.837 0-16 7.163-16 16v40c0 8.837 7.163 16 16 16z"
					/>
				</svg>
				<svg class="close" viewBox="0 0 384 512" width="100" title="times">
					<path
						d="M242.72 256l100.07-100.07c12.28-12.28 12.28-32.19 0-44.48l-22.24-22.24c-12.28-12.28-32.19-12.28-44.48 0L176 189.28 75.93 89.21c-12.28-12.28-32.19-12.28-44.48 0L9.21 111.45c-12.28 12.28-12.28 32.19 0 44.48L109.28 256 9.21 356.07c-12.28 12.28-12.28 32.19 0 44.48l22.24 22.24c12.28 12.28 32.2 12.28 44.48 0L176 322.72l100.07 100.07c12.28 12.28 32.2 12.28 44.48 0l22.24-22.24c12.28-12.28 12.28-32.19 0-44.48L242.72 256z"
					/>
				</svg>
			</label>
			<ul class="hamburger_options">
				<a href="http://"> <li>home</li> </a>
				<a href="http://"> <li>about</li> </a>
				<a href="http://"> <li>contact</li> </a>
			</ul>
		</div>
	</ul>
</nav>

<style lang="scss">
	.third_nav {
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
			// height: 3rem;
			gap: 5rem;
			& > * {
				display: flex;
			}
			.left_nav {
				flex: 1;
				img {
					width: 3rem;
					height: 3rem;
				}
			}
			.center_nav {
				flex: 1;
				justify-content: center;
			}

			.right_nav {
				position: relative;
				display: flex;
				flex-flow: column;
				flex: 1;
				justify-content: flex-end;
				align-items: flex-end;
				height: 100%;
				gap: 1rem;
				svg {
					width: 1.5rem;
					fill: #2a324b;
					cursor: pointer;
				}

				.close {
					display: none;
				}

				.menu {
					margin-top: 0.2rem;
				}

				.nav__checkbox {
					display: none;
				}
			}
		}

		.hamburger_options {
			position: absolute;
			top: 2rem;
			display: flex;
			flex-direction: column;
			gap: 2rem;
			align-items: center;
			margin: 1rem;
			transform: display 5s;
			li {
				list-style: none;
				display: none;
				&:first-child {
				}
			}

			a {
				text-decoration: none;
				color: inherit;
				font-size: 1.2rem;
			}
			svg {
				width: 1.5rem;
				fill: #2a324b;
			}
		}

		#nav__checkbox:checked ~ ul.hamburger_options li {
			display: block;
			animation-name: ease-in;
			animation-duration: 700ms;
			@keyframes ease-in {
				from {
					opacity: 0;
				}
				to {
					opacity: 1;
				}
			}
		
		}

		#nav__checkbox:checked ~ label.nav__checkbox.close {
			display: block;
			animation-name: ease-in;
			animation-duration: 700ms;
			@keyframes ease-in {
				from {
					opacity: 0;
				}
				to {
					opacity: 1;
				}
			}
		}

		#nav__checkbox:checked ~ label.right_nav.menu {
			display: none;
			animation-name: ease-in;
			animation-duration: 700ms;
			@keyframes ease-in {
				from {
					opacity: 0;
				}
				to {
					opacity: 1;
				}
			}
		}
	}
</style>
