<nav>
	<input type="checkbox" id="menu-toggle" class="menu-toggle" />
	<label for="menu-toggle" class="menu-icon">&#9776;</label>
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
		z-index: 100;
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		background-color: #fffdf1;
	}

	.menu-toggle {
		display: none;
	}

	.menu-icon {
		font-size: 30px;
		cursor: pointer;
		display: none;
	}

	ul {
		display: flex;
		justify-content: space-between;
		width: 100%;
		padding: 0;
		margin: 2em 3em;
	}

	li {
		list-style: none;
	}

	a {
		text-decoration: none;
		color: black;
		font-weight: 200;
		font-size: 20px;
	}

	@media (max-width: 768px) {
		.menu-icon {
			display: flex;
			margin: 1em;
			z-index: 100;
		}

		ul {
			display: flex;
			justify-content: start;
			gap: 7em;
			position: absolute;
			top: 60px;
			left: 0;
			background-color: #fffdf1;
			width: 100%;
			height: 100vh;
			flex-direction: column;
			align-items: center;
			display: none;
			margin: 0;
			padding-top: 3em;
		}

		ul li {
			padding: 10px 0;
		}

		/* When checkbox is checked, show the menu */
		.menu-toggle:checked + .menu-icon + ul {
			display: flex;
		}

		/* Optional: Add a little bit of transition effect */
		ul {
			transition: all 0.3s ease;
		}
	}
</style>
