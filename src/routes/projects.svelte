<script>
	import Button from '../lib/components/button/button.svelte';
</script>

<section class="container">
	<div class="content">
		<h1 class="header">PROJECTS</h1>
		<div class="groups">
			<div class="project">
				<img src="/assets/acmcsuf.svg" alt="Screenshot of project acmcsuf.com" />
				<div class="description">
					<h4 class="title">acmcsuf.com</h4>
					<Button text="SvelteKit" href="/disabled" disabled={true} />
					<Button text="TypeScript" href="/disabled" disabled={true} />
					<Button text="HTML5/CSS3" href="/disabled" disabled={true} />
				</div>
			</div>

			<div class="project">
				<img src="/assets/trello.svg" alt="Screenshot of project trello clone" />
				<div class="description">
					<h4 class="title">Trello Clone</h4>
					<Button text="React" href="/disabled" disabled={true} />
					<Button text="Next.js" href="/disabled" disabled={true} />
					<Button text="Node.js" href="/disabled" disabled={true} />
				</div>
			</div>

			<div class="project">
				<img src="/assets/gnome.svg" alt="Screenshot of gnome asset" />
				<div class="description">
					<h4 class="title">Gnome Asset</h4>
					<Button text="Unity" href="/disabled" disabled={true} />
					<Button text="C#" href="/disabled" disabled={true} />
					<Button text="Aseprite" href="/disabled" disabled={true} />
				</div>
			</div>
		</div>
	</div>
	<div class="extra">
		<Button text="More projects here!" href="https://github.com/karnikaavelumani" />
	</div>
</section>

<style>
	.container {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		width: 50%;
		margin: 0 auto;
		min-height: 100vh;
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
		margin-bottom: 1rem;
	}

	.groups {
		display: grid;
		grid-template-columns: 1fr 1fr;
		grid-gap: 2rem;
	}

	.project {
		border: solid;
		border-radius: 25px;
		padding: 2rem;
		width: 400px;
		height: 400px;
		display: flex;
		justify-content: center;
		position: relative;
	}

	img {
		max-width: 80%;
		max-height: 80%;
	}

	.description {
		position: absolute;
		bottom: 1rem;
		left: 1rem;
		padding: 0.5rem;
		border-radius: 8px;
	}

	.title {
		font-size: 20px;
		margin: 0;
	}

	.extra {
		display: flex;
		align-items: center;
		justify-content: center;
		margin-top: 2rem;
	}

	@media (max-width: 1024px) {
		.groups {
			grid-template-columns: 1fr;
		}
	}

	@media (max-width: 768px) {
		.project {
			width: 300px;
			height: 300px;
		}

		.header {
			font-size: 50px;
		}
	}
</style>
