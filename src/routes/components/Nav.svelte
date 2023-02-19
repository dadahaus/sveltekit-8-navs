<script>
	import { page } from '$app/stores';
</script>

<nav>
	<ul>
<<<<<<< HEAD
		<div class="left_nav">
			<li><a href="http://">home</a></li>
		</div>
		<div class="right_nav">
			<li><a href="http://">there</a></li>
			<li><a href="http://">yup</a></li>
			<li><a href="http://">first</a></li>
		</div>
=======
    <div class="left_nav">
      <a href="/"> <img src="src/assets/dribbble.svg" alt="logo" srcset=""> </a>

    </div>
		<div class="center_nav">
      <a href="http://"><li>menu</li></a>
      <a href="http://"><li>work</li></a>
      <a href="http://"><li>contact</li></a>
		</div>
    <div class="right_nav">
       <img src="src/assets/behance-2.svg" alt="logo" srcset=""> 
      <img src="src/assets/mail-1.svg" alt="logo" srcset="">
      <img src="src/assets/dribbble.svg" alt="logo" srcset="">
  
    </div>
>>>>>>> 3463c2a4597ac5cf8a02b438428273865e218084
	</ul>
</nav>

<style lang="scss">
	nav {
<<<<<<< HEAD
		padding: 2rem 5rem 2rem 5rem;
=======
padding: 2rem;
position: fixed;
bottom: 0rem;
width: 100%;
text-transform: uppercase;
>>>>>>> 3463c2a4597ac5cf8a02b438428273865e218084
		ul {
			display: flex;
			align-items: center;
			justify-content: space-between;
<<<<<<< HEAD
			gap: 5rem;
			text-transform: uppercase;
			.left_nav {
				flex-basis: 20%;
				justify-content: flex-start;
				img {
					width: 3rem;
					height: 3rem;
				}
			}
		
			.right_nav {
				display: flex;
				justify-content: flex-end;
				flex-basis: 30%;
				gap: 1rem;
				img {
					width: 3rem;
					height: 3rem;
				}
			}
=======
      gap: 5rem;
      .left_nav{
       flex: 1;
        img{
          width: var(--nav-item);
          height: var(--nav-item);
        }
      }
      .center_nav{
        flex: 1;

        display: flex;
        justify-content: space-evenly;
        gap: 1rem;
        // text-transform: uppercase;
        font-weight: 900;
      }
      .right_nav{
        display: flex;
        justify-content: flex-end;
        gap: 1rem;
        flex: 1;
        // gap: 1rem;
        img{
          width: var(--nav-item);
          height: var(--nav-item);
        }
        
      }
>>>>>>> 3463c2a4597ac5cf8a02b438428273865e218084
		}
	}
</style>
