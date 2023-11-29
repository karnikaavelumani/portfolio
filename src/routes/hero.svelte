<section class="hero__component">
	<div class="hero__container">
		<div class="hero__content">
			<div class="hero__image">
				<img src="/assets/karni-hero.svg" alt="Drawing of Karni in manga style art" />
			</div>
			<div class="hero__title">
				<h1 class="hero__title__description">Welcome to my website!</h1>
			</div>
		</div>
		<div class="hero__bio">
			<p class="hero__bio__description">
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
		border: 2px solid #000;
		display: grid;
		align-items: center;
		max-width: 100%;
		margin: 0 auto;
	}

	.hero__content {
		display: grid;
		grid-template-columns: 3fr 1fr;
		align-items: center;
	}

	.hero__title {
		display: grid;
		justify-self: center;
		align-items: center;
		max-width: 100%;
	}

	.hero__image img {
		max-width: 100%;
		position: relative;
	}

	.hero__title h1 {
		background-color: #fff;
		border: 2px solid #000;
		border-radius: 50%;
		max-width: 5rem;
		width: 100%;
	}

	.hero__title__description {
		display: flex;
		justify-content: center;
		align-items: center;
		text-align: center;
		position: absolute;
		font-size: 15px;
		z-index: 10;
		right: 1rem;
		padding: 2rem;
		margin-right: 1rem;
	}

	.hero__bio {
		display: flex;
		justify-content: center;
		align-items: center;
		margin: 1em 2em;
		background: white;
	}

	.hero__bio__description {
		display: flex;
		text-align: center;
		font-size: 10px;
		font-weight: 600;
		max-width: 90%;
		padding: 2em 2em;
		border: 2px solid #000;
	}

	@media screen and (min-width: 768px) {
		.hero__title h1 {
			max-width: 10rem;
		}

		.hero__title__description {
			font-size: 35px;
			padding: 8rem 3rem;
			right: 2rem;
		}

		.hero__bio__description {
			font-size: 15px;
		}
	}

	@media screen and (min-width: 1024px) {
		section {
			max-width: 1024px;
		}

		.hero__title h1 {
			max-width: 10rem;
		}

		.hero__title__description {
			font-size: 40px;
			padding: 10rem 5rem;
			right: 2rem;
		}

		.hero__bio__description {
			font-size: 20px;
			padding: 2rem 2rem;
		}
	}
</style>
