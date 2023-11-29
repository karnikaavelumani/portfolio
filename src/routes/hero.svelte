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
				in frontend development. This website reflects the world inside my head, and I aim to bring
				it to life through my coding skills. Check out all the pages to learn more about me!
			</p>
		</div>
	</div>
</section>

<style>
	section {
		background-color: #fff;
		display: grid;
		align-items: center;
		max-width: 100%;
		margin: 0 auto;
	}

	.hero__content {
		display: grid;
		grid-template-columns: 3fr 1fr;
	}

	.hero__title {
		display: grid;
		justify-self: center;
		align-items: center;
		max-width: 100%;
	}

	.hero__content {
		position: relative;
	}

	.hero__image img {
		max-width: 100%;
		position: relative;
	}

	.hero__title h1 {
		background-color: #fff;
		border: 2px solid #000;
		border-radius: 50%;
		height: 20vh;
		width: 5vw;
	}

	.hero__description {
		display: flex;
		justify-content: center;
		align-items: center;
		text-align: center;
		position: absolute;
		font-weight: 700;
		font-size: 20px;
		z-index: 10;
		left: 65%;
		padding: 0 2em;
	}

	.hero__bio {
		display: flex;
		justify-content: center;
		align-items: center;
		margin: 1em 2em;
		background: white;
	}

	.hero__bio-description {
		display: flex;
		text-align: center;
		font-size: 10px;
		font-weight: 700;
		max-width: 90%;
		padding: 2em 2em;
		border: 2px solid #000;
	}

	@media screen and (min-width: 768px) {
		.hero__title h1 {
			height: 40vh;
			width: 5vw;
		}

		.hero__description {
			font-size: 40px;
			left: 70%;
		}

		.hero__bio-description {
			font-size: 15px;
		}
	}

	@media screen and (min-width: 1024px) {
		section {
			max-width: 1024px;
		}

		.hero__title h1 {
			height: 45vh;
			width: 5vw;
		}

		.hero__description {
			font-size: 40px;
			left: 65%;
		}

		.hero__bio-description {
			font-size: 20px;
		}
	}
</style>
