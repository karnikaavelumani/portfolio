<section class="page2__component">
	<div class="page2__container">
		<div class="page2__first__block">
			<img
				src="/assets/karni-meme.svg"
				alt="Drawing of Karni as a meme in One Punch Man art style"
			/>
			<div class="first__block__content">
				<h1 class="first__block__content__text">But, those jobs weren't clicking for me.</h1>
			</div>
		</div>
		<div class="page2__second__block">
			<div class="second__block__content">
				<p class="second__block__content__text">
					I'm passionate about crafting experiences through interactive interfaces and building
					meaningful relationships within the developer community. Programming is my calling,
					blending creativity with technical expertise to empower and inspire others.
				</p>
			</div>
			<img
				src="/assets/karni-determined.svg"
				alt="Drawing of Karni determined in manga art style"
			/>
		</div>
		<div class="page2__third__block">
			<div class="third__block__content">
				<h1 class="third__block__content__text">And that's exactly what my goal is!</h1>
			</div>
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
		max-width: 1024px;
	}

	.page2__container {
		display: grid;
	}

	.page2__first__block {
		display: grid;
		grid-template-columns: 1fr 1fr;
		justify-self: end;
		align-self: start;
		max-width: 80%;
		height: 25rem;
		background-color: #000;
		border: 2px solid #000;
		padding: 0 3rem;
		margin-bottom: 2rem;
	}

	.page2__first__block img {
		display: grid;
		justify-self: end;
		align-self: end;
		max-width: 80%;
	}

	.first__block__content {
		display: grid;
		justify-self: center;
		align-self: center;
		text-align: center;
		background: #fff;
		border-radius: 50%;
		max-width: 20rem;
		width: 100%;
	}

	.first__block__content__text {
		color: #000;
		font-size: 1.5rem;
		font-weight: 700;
		text-align: center;
		padding: 3rem 5rem;
	}

	.page2__second__block {
		display: grid;
		grid-template-columns: 1fr 1fr;
		justify-self: end;
		align-self: end;
		max-width: 80%;
		height: 25rem;
		background-color: #fff;
		border: 2px solid #000;
		padding: 0 0 3rem 3rem;
		margin-bottom: 2rem;
	}

	.second__block__content {
		display: grid;
		justify-self: center;
		align-self: center;
		text-align: center;
		max-width: 30rem;
		width: 100%;
	}

	.second__block__content__text {
		color: #000;
		font-size: 1.25rem;
		font-weight: 700;
		text-align: center;
		padding: 0.1rem;
	}

	.page2__second__block img {
		display: grid;
		justify-self: end;
		align-self: end;
		max-width: 99%;
	}

	.page2__third__block {
		display: grid;
		grid-template-columns: 1fr;
		justify-self: end;
		align-self: end;
		/* max-width: 100%; */
		height: 25rem;
		background-color: #fff;
		border: 2px solid #000;
		padding: 0 0 3rem 3rem;
		margin-bottom: 2rem;
	}

	.third__block__content {
		display: grid;
		justify-self: center;
		align-self: center;
		text-align: center;
		/* max-width: 100%; */
	}

	/* .third__block__content__text {
		color: #000;
		font-size: 1.25rem;
		font-weight: 700;
		text-align: center;
		padding: 0.1rem;
	} */
</style>
