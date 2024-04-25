<script lang="ts">
	// TODO: Add button for contacts
	const contact = ['email', 'phone', 'linkedin', 'discord', 'whatsapp'];
	const socials = [
		{ name: 'github', url: 'https://github.com/karnikaavelumani' },
		{ name: 'tiktok', url: 'https://www.tiktok.com/@demonic__goat' },
		{ name: 'mastodon', url: 'https://mastodon.social/@demonicgoat' },
		{ name: 'pinterest', url: 'https://www.pinterest.com/karnivelu/' },
		{ name: 'reddit', url: 'https://www.reddit.com/user/Demonic__Goat' },
		{ name: 'youtube', url: 'https://www.youtube.com/@karnikaavelumani' },
		{ name: 'facebook', url: 'https://www.facebook.com/karnikaa.velumani' },
		{ name: 'figma', url: 'https://www.figma.com/@karni' }
	];
</script>

<footer>
	<div class="container">
		<div class="contact_container">
			<p class="contact_title">Get in touch</p>
			<ul class="contact">
				{#each contact as contactPath (contactPath)}
					<li>
						<a href={contactPath} target="_blank" rel="noopener noreferrer">
							<img src={`/assets/${contactPath}.svg`} alt={contactPath.slice(1)} />
						</a>
					</li>
				{/each}
			</ul>
		</div>

		<div class="socials_container">
			<p class="social_title">Stay connected</p>
			<ul class="socials">
				{#each socials as social (social.name)}
					<li>
						<a href={social.url} target="_blank" rel="noopener noreferrer">
							<img src={`/assets/${social.name}.svg`} alt={social.name} />
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
		display: grid;
		justify-self: center;
		align-self: center;
		background-color: white;
		max-width: 1024px;
		padding: 1rem 0;
		margin: 0 auto;
		border: 2px solid #000;
	}

	.container {
		display: grid;
		justify-self: center;
		align-self: center;
	}

	.contact_container {
		display: grid;
		justify-self: center;
		align-self: center;
	}

	.socials,
	.contact {
		display: flex;
		list-style: none;
		padding: 0;
	}

	.socials li,
	.contact li {
		margin: 0 0.5rem;
	}

	.socials img,
	.contact img {
		width: 3rem;
	}

	.social_title,
	.contact_title {
		display: grid;
		justify-self: center;
		align-self: center;
		text-align: center;
		margin: 0;
	}

	.copyright_title {
		display: grid;
		justify-self: center;
		align-self: center;
		text-align: center;
		margin: 0;
	}
</style>
