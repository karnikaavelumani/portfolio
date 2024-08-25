<nav>
	<div class="container">
		<ul class="container_list">
			<li><a href="/">Home</a></li>
			<li><a href="/diary">Diary</a></li>
			<li><a href="/studio">Studio</a></li>
			<li><a href="/projects">Projects</a></li>
		</ul>
	</div>
</nav>

<style>
	nav {
		display: flex;
		justify-content: center;
		align-items: center;
	}

	.container {
		background-color: white;
		border: 2px solid black;
		width: 100%;
		max-width: 1024px;
		position: fixed;
		top: 0;
		z-index: 100;
	}

	.container_list {
		display: flex;
		list-style-type: none;
		justify-content: space-around;
		margin: 1rem;
		padding: 0;
	}

	nav li {
		/* padding: 0 1rem; */
	}

	nav a {
		text-decoration: none;
		color: black;
	}

	nav a:hover {
		color: #f00;
	}
</style>
