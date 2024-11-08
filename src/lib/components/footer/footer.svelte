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
			<!-- <p class="social_title">Stay connected</p> -->
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
		margin: 0;
		width: 100%;
	}
</style>
