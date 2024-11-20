<script>
	import Hero from './hero.svelte';
	import About from './about.svelte';
	import Experience from './exp.svelte';
	import Projects from './projects.svelte';
	import Skills from './skills.svelte';
</script>

<svelte:head>
	<title>Karni's Portfolio</title>
</svelte:head>

<div id="hero">
	<Hero />
</div>

<div id="about">
	<About />
</div>

<div id="experience">
	<Experience />
</div>

<div id="projects">
	<Projects />
</div>

<div id="skills">
	<Skills />
</div>
