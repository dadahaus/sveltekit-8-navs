<script>
	import { page } from '$app/stores';
</script>

<nav>
	<ul>
    <div class="left_nav">
      <a href="/"> <img src="src/assets/dribbble.svg" alt="logo" srcset=""> </a>

    </div>
		<div class="center_nav">
		</div>
    <div class="right_nav">
      <img src="src/assets/behance-2.svg" alt="logo" srcset="">
      <img src="src/assets/mail-1.svg" alt="logo" srcset="">
      <img src="src/assets/dribbble.svg" alt="logo" srcset="">
  
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
      .left_nav{
        flex-basis: 10%;
        img{
          width: 3rem;
          height: 3rem;
        }
      }
      .center_nav{
        flex-basis:80%;
        display: flex;
        justify-content: space-evenly;
        // text-transform: uppercase;
        font-weight: 900;
      }
      .right_nav{
        display: flex;
        justify-content: center;
        flex-basis: 10%;
        img{
          width: 3rem;
          height: 3rem;
        }
        
      }
		}
	}
</style>
