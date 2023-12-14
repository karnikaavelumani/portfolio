<section class="page1__component">
	<div class="page1__container">
		<div class="page1__content">
			<img src="/assets/karni-hero.svg" alt="Drawing of Karni in manga style art" />
			<div class="page1__title">
				<h1 class="page1__title__description">Welcome to my website!</h1>
			</div>
		</div>
		<div class="page1__bio">
			<p class="page1__bio__description">
				Hello! Nice to meet you. My name is Karnikaa Velumani. I am a software engineer specializing
				in frontend development. This website reflects the world inside my head, and I aim to bring
				it to life through my programming skills. Check out all the pages to learn more about me!
			</p>
		</div>
		<div class="page1__experience">
			<div class="page1__experience__job1">
				<p class="page1__experience__job1__description">Originally, I worked as a STEAM teacher!</p>
				<img
					src="/assets/teaching-job.svg"
					alt="Drawing of Karni correcting a math test in manga style art"
				/>
			</div>
			<!-- <div class="page1__experience__job2">
				<p class="page1__experience__job2__description">
					Following that, I undertook the role as a Data Analyst intern.
				</p>
				<img
					src="/assets/analyst-intern.svg"
					alt="Drawing of laptop with analytics on the screen in manga style art"
				/>
			</div> -->
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

	.page1__content {
		display: grid;
		grid-template-columns: 3fr 1fr;
		align-items: center;
	}

	.page1__content img {
		max-width: 100%;
		position: relative;
	}

	.page1__title {
		display: grid;
		justify-self: center;
		align-items: center;
		max-width: 100%;
	}

	.page1__title h1 {
		background-color: #fff;
		border: 2px solid #000;
		border-radius: 50%;
		max-width: 5rem;
		width: 100%;
	}

	.page1__title__description {
		display: flex;
		justify-content: center;
		align-items: center;
		text-align: center;
		position: absolute;
		font-size: 15px;
		z-index: 10;
		padding: 15% 2%;
		right: 5vw;
	}

	.page1__bio {
		display: flex;
		justify-content: center;
		align-items: center;
		margin: 0 1em;
		background: white;
	}

	.page1__bio__description {
		display: flex;
		text-align: center;
		font-size: 10px;
		font-weight: 600;
		max-width: 90%;
		padding: 1.5em;
		border: 2px solid #000;
	}

	.page1__experience {
		display: grid;
		grid-template-columns: 1fr 1fr;
		gap: 1em;
		margin: 0 1em;
	}

	.page1__experience__job1 {
		display: grid;
		grid-template-columns: 1fr 3fr;
		align-items: center;
		border: 2px solid #000;
	}

	.page1__experience__job1 img {
		max-width: 100%;
		position: relative;
		grid-column: 2;
	}

	.page1__experience__job1__description {
		display: flex;
		justify-content: center;
		align-items: center;
		text-align: center;
		position: absolute;
		max-width: 5rem;
		width: 100%;
		font-size: 15px;
		z-index: 10;
		left: 18vw;
	}

	@media screen and (min-width: 500px) {
		.page1__title__description {
			font-size: 20px;
			padding: 15% 5%;
			right: 10vw;
		}
	}

	@media screen and (min-width: 768px) {
		.page1__title h1 {
			max-width: 10rem;
		}

		.page1__title__description {
			font-size: 35px;
			padding: 15% 5%;
			right: 5%;
		}

		.page1__bio__description {
			font-size: 15px;
		}

		.page1__experience {
			margin: 0 2em;
			margin-bottom: 1em;
		}
	}

	@media screen and (min-width: 1024px) {
		section {
			max-width: 1024px;
		}

		.page1__title h1 {
			max-width: 10rem;
		}

		.page1__title__description {
			font-size: 40px;
			padding: 100% 50%;
			right: 100%;
			position: relative;
		}

		.page1__bio__description {
			font-size: 20px;
			padding: 2rem;
		}

		.page1__experience {
			margin: 0 2em;
			margin-bottom: 1em;
		}
	}
</style>
