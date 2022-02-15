<script>
	export let name;
</script>
<header id="top">
	<div class="headerLeft">
		<ul>
			<li><a href="#top">Page One</a></li>
			<li><a href="#middle">Page Two</a></li>
			<li><a href="#bottom">Page Three</a></li>
	
		</ul>
	</div>
	
	<input id="headerInpt" type="text" placeholder="Searc">



	
	<div class="headerRight">
		<img src="./src/brandon.png" alt="undefine" id="profil">
		<a id="headerDot" href="#top">...</a>
	</div>
</header>
<main id="middle">
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
	<div class="content">
		<div class="contentBox">
			<div class="imgBox">
				<img src="https://media.istockphoto.com/vectors/coding-and-development-concept-vector-id590173260?s=612x612"width="95%" alt="">
			</div>
			<div class="textBox">
				<p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nobis, consequatur.</p>
			</div>
		</div>

		<div class="contentBox">
			<div class="imgBox">
				<img src="https://media.istockphoto.com/vectors/coding-and-development-concept-vector-id590173260?s=612x612"width="95%" alt="">
			</div>
			<div class="textBox">
				<p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nobis, consequatur.</p>
			</div>
		</div>

		<div class="contentBox">
			<div class="imgBox">
				<img src="https://media.istockphoto.com/vectors/coding-and-development-concept-vector-id590173260?s=612x612"width="95%" alt="">
			</div>
			<div class="textBox">
				<p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nobis, consequatur.</p>
			</div>
		</div>
	</div>
</main>
<footer id="bottom">
	<div class="textBox">
		<h2>Gmail:email@gmail.com</h2>
		<h2>Phone:1234567891011</h2>

	</div>

</footer>

<style>
	
	.content{
		margin-top: 150px;
		display: flex;
		justify-content: center;
		align-items: center;
		width: 100%;
		

	}
	.contentBox{
		width: 400px;
		height: 500px;
		background-color:#ff3e00;
		border: 1px solid  rgba(128, 128, 128, 0.87);
		border-radius: 16px;
		box-shadow: -3px 20px 40px 15px grey;
		margin: auto auto;
	}
	.imgBox{
		margin-top: 10px;
	}
	.textBox{
		margin-top: 10px;
		border-top: 1px solid rgba(128, 128, 128, 0.87);
		color:wheat;
	}
	header{
		margin: 0;
		padding: 0;
		display:flex;
		flex-direction: row;
		align-items: center;
		justify-content: space-between;
		max-width: 100%;
		height: 100px;
		font-family: monospace;
		color: #ff3e00;
		
	}
	.headerLeft{
		display: flex;
		justify-content: flex-start;
		align-items: center;
		width:30%;

	}
	.headerRight{
		display: flex;
		align-items: center;
		justify-content: flex-end;
		padding-right: 10px;
		margin-right: 10px;
		width:30%;
	}
	ul{
		display: flex ;
		list-style-type: none;
	}
	ul li{
		text-align: center;
		font-family: monospace;
		font-size:1rem;
		line-height: 18px;
		border-right: 1px solid lightblue;
		padding-right:10px ;
		
	}
	a{
		color:#ff3e00;
		text-decoration: none;
	}
	li:hover{
		border-bottom: 1px solid gray;
		color: gray;
	}
	#headerInpt{
		width: 300px;
		height: 30px;
		display: flex;
		justify-content: center;
		align-items: center;
		border-radius: 8px;
		border: 1px solid #ff3e00;
		background-color: rgba(255, 2555, 222, 0);
	}
	#headerDot{
		margin-left: 20px;
		margin-right: 20px;
		font-size: 1rem;
		font-weight: 900;
	}
	main {
		width: 100vw;
		text-align: center;
		margin-top: 8rem;
		margin-bottom: 15rem;
		max-width: 240px;
		background-color: white;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}
	footer{
		display: flex;
		justify-content: center;
		align-items: center;
		width: 100vw;
		height: 300px;
		background-color: #ff3e00;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
		header{
			max-width: none;
			
		}
	}
</style>