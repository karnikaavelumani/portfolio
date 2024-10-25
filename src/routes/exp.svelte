<section class="container">
	<div class="content">
		<h1 class="header">EXPERIENCE</h1>
		<div class="positions">
			<div class="designer">
				<h2 class="title">UI/UX Designer</h2>
				<p class="description">
					Freelance UI/UX Designer for Edaters.gg, a platform that connects gamers through a shared,
					interest-based online dating experience. Responsible for developing reward iconography and
					homepage assets using Figma, with design implementation executed in collaboration with a
					team of two, leveraging HTML/CSS within the Angular.js framework.
				</p>
				<button class="button">Website</button>
				<button class="button">Case Study</button>
			</div>
			<div class="analyst">
				<h2 class="title">Data Analyst</h2>
				<p class="description">tbd</p>
			</div>
			<div class="teacher">
				<h2 class="title">STEAM Teacher</h2>
				<p class="description">tbd</p>
			</div>
		</div>
	</div>
</section>

<style>
	/* create a drop down for each of the positions */
	.container {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		height: 100vh;
		width: 50%;
		margin: 0 auto;
	}

	.content {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		justify-content: center;
	}

	.header {
		font-size: 75px;
		font-weight: 400;
		margin: 0;
	}

	.positions {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.designer,
	.analyst,
	.teacher {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		margin: 20px 0;
		padding: 20px;
		border-radius: 10px;
		background-color: var(--acm-odd);
	}

	.title {
		font-size: 40px;
		font-weight: 400;
		margin: 0;
	}

	.description {
		font-size: 20px;
		font-weight: 300;
		margin: 10px 0;
	}

	.button {
		margin: 10px 0;
		padding: 10px 20px;
		border: none;
		border-radius: 5px;
		background-color: var(--acm-even);
		color: var(--acm-odd);
		font-size: 20px;
		font-weight: 300;
		cursor: pointer;
	}

	.button:hover {
		background-color: var(--acm-odd);
		color: var(--acm-even);
	}

	.button:active {
		transform: scale(0.95);
	}

	.button:focus {
		outline: none;
	}
</style>
