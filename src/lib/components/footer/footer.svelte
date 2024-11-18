<script lang="ts">
	const contacts = [
		{ name: 'email', url: 'mailto:karnivelu@outlook.com' },
		{ name: 'phone', url: 'tel:+1-714-609-2078' },
		{ name: 'linkedin', url: 'https://linkedin/in/karnivelu' },
		{ name: 'github', url: 'https://github.com/karnikaavelumani' }
	];
</script>

<footer>
	<div class="container">
		<div class="content">
			<p class="go_back">Back to the top!</p>
			<ul class="contacts">
				{#each contacts as contact (contact.name)}
					<li>
						<a href={contact.url} target="_blank" rel="noopener noreferrer">
							<img src={`/assets/${contact.name}.svg`} alt={contact.name} />
						</a>
					</li>
				{/each}
			</ul>
		</div>

		<p class="copyright_title">&copy; 2024 Karnikaa Velumani</p>
	</div>
</footer>

<style>
	footer {
		display: flex;
		align-items: center;
		justify-content: center;
		background-color: black;
		border-radius: 100px 100px 0 0;
		width: 100%;
	}

	.container {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		width: 50%;
	}

	ul {
		display: flex;
		gap: 1em;
		padding: 0;
		margin: 0;
	}

	li {
		border: 1px solid white;
		border-radius: 50%;
		list-style: none;
	}

	img {
		width: 35px;
		height: 35px;
		padding: 10px;
	}

	p {
		color: white;
	}
</style>
