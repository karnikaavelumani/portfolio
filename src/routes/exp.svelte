<script>
	import Button from '../lib/components/button/button.svelte';
</script>

<section class="container">
	<div class="content">
		<h1 class="header">EXPERIENCE</h1>

		<div class="tab">
			<input type="checkbox" name="exp-1" id="cb1" />
			<label for="cb1" class="tab__label"> Freelance UI/UX Designer </label>
			<hr />
			<div class="tab__content">
				<div class="extra">
					<p class="time"><i><b>Sept 2024 - Present</b></i></p>
					<p class="location"><i><b>Remote</b></i></p>
				</div>
				<p class="description">
					Freelance UI/UX Designer for Edaters.gg, a platform that connects gamers through a shared,
					interest-based online dating experience. Responsible for developing reward iconography and
					homepage assets using Figma, with design implementation executed in collaboration with a
					team of two, leveraging HTML/CSS within the Angular.js framework.
				</p>
				<Button text="Website" href="https://edaters.gg" />
				<Button text="Case Study" href="/disabled" disabled={true} />
			</div>
		</div>

		<div class="tab">
			<input type="checkbox" name="exp-2" id="cb2" />
			<label for="cb2" class="tab__label"> Open Source Software Co-Team Lead </label>
			<hr />
			<div class="tab__content">
				<div class="extra">
					<p class="time"><i><b>Jun 2023 - Jun 2024</b></i></p>
					<p class="location"><i><b>Fullerton, CA</b></i></p>
				</div>
				<p class="description">
					Co-Team Lead for the Open Source Software (OSS) team at ACM, CSUF. Co-founded and led an
					open-source initiative through weekly, in-depth workshops designed to teach and inspire
					dedicated students. Oversaw diverse team projects across skill levels, programming
					languages, and industry domains, fostering an agile approach to project development and
					collaboration.
				</p>
				<Button text="Video" href="https://www.youtube.com/watch?v=GyU0s2McDgw" />
				<Button text="LinkedIn" href="https://www.linkedin.com/company/acmcsufoss/" />
				<Button text="Projects" href="https://github.com/acmcsufoss/" />
			</div>
		</div>

		<div class="tab">
			<input type="checkbox" name="exp-3" id="cb3" />
			<label for="cb3" class="tab__label">
				Association for Computing Machinery CSUF President
			</label>
			<hr />
			<div class="tab__content">
				<div class="extra">
					<p class="time"><i><b>May 2022 - May 2023</b></i></p>
					<p class="location"><i><b>Fullerton, CA</b></i></p>
				</div>
				<p class="description">
					President of the Association for Computing Machinery (ACM) chapter at CSUF, leading the
					largest computer science club on campus with over 2,000 students. Directed impactful
					strategies in weekly board meetings, planning, designing, and executing initiatives.
					Oversaw and supported the development of accessible workshops for all skill levels.
					Represented the club at campus events, actively participating and engaging as ACM’s lead
					representative.
				</p>
				<Button text="Website" href="https://acmcsuf.com/" />
			</div>
		</div>

		<div class="tab">
			<input type="checkbox" name="exp-4" id="cb4" />
			<label for="cb4" class="tab__label"> Data Analyst Intern </label>
			<hr />
			<div class="tab__content">
				<div class="extra">
					<p class="time"><i><b>May 2022 - Aug 2022</b></i></p>
					<p class="location"><i><b>Orange, CA</b></i></p>
				</div>
				<p class="description">
					Data Analyst Intern at MSI Surfaces, a leading floor tile company, leveraging Sisense BI
					to develop interactive dashboards that streamline shipment data analytics and identify
					packaging errors. Responsible for extracting and refining data in Excel for improved
					clarity, and managing a Sisense deployment migration from Windows to Linux, performing
					rigorous audits to ensure the functionality of all key assets, models, and dashboards,
					while maintaining seamless user access.
				</p>
				<Button text="PowerPoint Presentation" href="/disabled" disabled={true} />
			</div>
		</div>

		<div class="tab">
			<input type="checkbox" name="exp-5" id="cb5" />
			<label for="cb5" class="tab__label"> Math/STEAM Academy Teacher </label>
			<hr />
			<div class="tab__content">
				<div class="extra">
					<p class="time"><i><b>Dec 2020 - May 2022</b></i></p>
					<p class="location"><i><b>Fullerton, CA</b></i></p>
				</div>
				<p class="description">
					Math and STEAM Teacher for Innovation Academy, an afterschool program, specializing in the
					development of interactive activities and lesson plans focused on robotics (Arduino, EV3,
					NXT) and programming (C, Lua, Python) to foster student engagement and mastery.
					Responsible for designing and delivering instructional materials and study sessions
					tailored to students with varying levels of computer science knowledge, effectively
					enhancing critical thinking skills.
				</p>
				<Button text="Website" href="https://www.myinnoacademy.com/" />
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

	.tab {
		position: relative;
		margin-top: 10px;
	}
	.tab input {
		position: absolute;
		opacity: 0;
		z-index: -1;
	}
	.tab__content {
		max-height: 0;
		overflow: hidden;
		transition: all 0.35s;
	}
	.tab input:checked ~ .tab__content {
		max-height: 10rem;
	}

	.tab__label {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		font-size: 26px;
		font-weight: 400;
		cursor: pointer;
	}

	.tab__label::after {
		content: '+';
		text-align: center;
		font-size: 30px;
		font-weight: 200;
		transform: rotate(90deg);
		transition: all 0.35s;
	}

	.tab input:checked + .tab__label::after {
		transform: rotate(45deg);
	}

	.description {
		font-size: 16px;
		font-weight: 300;
		margin: 0;
	}

	.extra {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		font-size: 14px;
	}

	.time,
	.location {
		margin: 0;
		margin-bottom: 2px;
		padding: 0;
	}

	/* @media (max-width: 1024px) {
		.container {
			width: 70%;
		}

		.header {
			font-size: 60px;
		}

		.tab__label {
			font-size: 22px;
		}

		.description {
			font-size: 14px;
		}

		.extra {
			font-size: 12px;
		}
	}

	@media (max-width: 768px) {
		.container {
			width: 90%;
		}

		.header {
			font-size: 55px;
		}

		.tab__label {
			font-size: 20px;
		}

		.description {
			font-size: 14px;
		}

		.extra {
			font-size: 12px;
		}
	}

	@media (max-width: 480px) {
		.header {
			font-size: 50px;
		}

		.tab__label {
			font-size: 20px;
		}

		.description {
			font-size: 14px;
		}

		.extra {
			font-size: 12px;
		}
	} */
</style>
