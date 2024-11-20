<script>
	import Button from '$lib/components/button/button.svelte';
	import { text } from '@sveltejs/kit';
</script>

<section class="container">
	<div class="content">
		<h1 class="header">SKILLS</h1>
		<div class="groups">
			<h2 class="subheader">Languages</h2>
			<div class="skills">
				<Button text="JavaScript" href="/disabled" disabled={true} />
				<!-- <Button
					text="JavaScript"
					href="/disabled"
					disabled={true}
					imageSrc="/assets/skills/javascript.svg"
					imageAlt="JavaScript logo"
				/> -->
				<Button text="TypeScript" href="/disabled" disabled={true} />
				<Button text="HTML5/CSS3" href="/disabled" disabled={true} />
				<Button text="Python" href="/disabled" disabled={true} />
				<Button text="C++" href="/disabled" disabled={true} />
				<Button text="R Studio" href="/disabled" disabled={true} />
				<Button text="SQL" href="/disabled" disabled={true} />
				<Button text="Golang" href="/disabled" disabled={true} />
				<Button text="Java" href="/disabled" disabled={true} />
				<Button text="C#" href="/disabled" disabled={true} />
			</div>
		</div>

		<div class="groups">
			<h2 class="subheader">Tools</h2>
			<div class="skills">
				<Button text="Git/GitHub" href="/disabled" disabled={true} />
				<Button text="AWS" href="/disabled" disabled={true} />
				<Button text="Node.js" href="/disabled" disabled={true} />
				<Button text="Deno" href="/disabled" disabled={true} />
				<Button text="Svelte/SvelteKit" href="/disabled" disabled={true} />
				<Button text="React/Next.js" href="/disabled" disabled={true} />
				<Button text="Figma" href="/disabled" disabled={true} />
				<Button text="Powershell" href="/disabled" disabled={true} />
				<Button text="Sisense BI" href="/disabled" disabled={true} />
				<Button text="Vercel" href="/disabled" disabled={true} />
				<Button text="Netlify" href="/disabled" disabled={true} />
				<Button text="Supabase" href="/disabled" disabled={true} />
			</div>

			<div class="groups">
				<h2 class="subheader">Certifications</h2>
				<div class="skills">
					<Button text="AWS Certified Cloud Practitioner" href="/disabled" disabled={true} />
				</div>
			</div>
		</div>
	</div>
</section>

<style>
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

	h2 {
		margin-top: 1em;
		margin-bottom: 0;
	}
</style>
