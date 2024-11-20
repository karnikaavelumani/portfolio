<nav>
	<ul>
		<li><a href="#about">ABOUT</a></li>
		<li><a href="#experience">EXPERIENCE</a></li>
		<li><a href="#projects">PROJECTS</a></li>
		<li><a href="#skills">SKILLS</a></li>
		<li><a href="#resume">RESUME</a></li>
	</ul>
</nav>

<style>
	nav {
		display: flex;
		justify-content: center;
		z-index: 100;
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		background-color: #fffdf1;
	}

	ul {
		display: flex;
		justify-content: space-between;
		width: 100%;
		margin: 2em 3em;
	}

	li {
		display: flex;
		align-items: center;
		justify-content: space-between;
		list-style: none;
	}

	a {
		text-decoration: none;
		color: black;
		font-weight: 200;
		font-size: 20px;
	}

	@media (max-width: 768px) {
		ul {
			margin: 1em 2em;
		}

		a {
			font-size: 16px;
		}
	}

	@media (max-width: 425px) {
		ul {
			margin: 1em 1em;
		}

		a {
			font-size: 14px;
		}
	}
</style>
