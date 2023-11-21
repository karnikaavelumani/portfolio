<section class="hero__component">
	<div class="hero__container">
		<div class="hero__content">
			<div class="hero__image">
				<img src="/assets/karni-hero.svg" alt="Drawing of Karni in manga style art" />
			</div>
			<div class="hero__title">
				<h1 class="hero__description">Welcome to my website!</h1>
			</div>
		</div>
		<div class="hero__bio">
			<p class="hero__bio-description">
				Hello! Nice to meet you. My name is Karnikaa Velumani. I am a software engineer specializing
				in frontend development. This is just a random blurb where I'll write a little bit about
				myself so I still need to think about what I'll write.
			</p>
		</div>
	</div>
</section>

<style>
	section {
		background-color: #fff;
		display: grid;
		justify-self: center;
		align-items: center;
		max-width: 100%;
		height: 100%;
		margin: 0 auto;
	}

	.hero__content {
		display: grid;
		grid-template-columns: 1fr 1fr;
	}

	.hero__title {
		display: grid;
		justify-self: center;
		align-items: center;
		max-width: 100%;
	}

	.hero__image img {
		max-width: 100%;
		/* z-index: -999; */
	}

	.hero__title h1 {
		font-weight: 700;
	}

	.hero__bio {
		position: relative;
		background: rgba(255, 255, 255, 0.7);

		border: 2px solid #000;
		max-width: 90%;
		margin: -2em 2em;
		z-index: 999;
		/* z-index: 999; */
	}

	.hero__bio-description {
		font-weight: 700;
		margin: 2em 2em;
	}

	@media screen and (min-width: 1024px) {
		section {
			max-width: 1024px;
		}
	}
</style>
