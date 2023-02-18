<script>
	import { page } from '$app/stores';
</script>

<nav class="fourth_nav">
	<div class="left_nav">
		<input type="checkbox" id="nav__checkbox" class="nav__checkbox" />
		<label for="nav__checkbox" class="nav__toggle">
			<li>menu</li>
		</label>
		<ul class="menu_options">
			<a href="http://"> <li>home</li> </a>
			<a href="http://"> <li>about</li> </a>
			<a href="http://"> <li>contact</li> </a>
		</ul>
	</div>
	<div class="right_nav">
		<a href="/"> <img src="src/assets/dribbble.svg" alt="logo" srcset="" /> </a>
	</div>
</nav>

<style lang="scss">
	.fourth_nav {
		display: flex;
		padding: 1rem 2rem 1rem 2rem;
		position: fixed;
		width: 100%;
		top: 0;
		text-transform: uppercase;
		font-weight: 700;
		justify-content: center;

		.left_nav {
			flex-basis: 50%;
			position: relative;
			display: flex;
			flex-flow: column;


			align-items: flex-start;
			justify-content: center;
			height: 2rem;

			gap: 1rem;
      li{
        cursor: pointer;

      }
			input {
				height: 100%;
			}
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

			.menu_options {
				position: absolute;
				top: 2rem;
				display: flex;
				flex-direction: column;
				gap: 2rem;
				align-items: flex-start;
				margin-top: 2rem;
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

			}

			#nav__checkbox:checked ~ ul.menu_options li {
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
		.right_nav {
			// position: relative;
			flex-basis: 50%;

			img {
				// top: 2rem;
				right: 2rem;
				position: absolute;
				width: 2rem;
				height: 2rem;
			}
		}
	}
</style>
