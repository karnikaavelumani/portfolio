<script>
	import Spacing from '$lib/spacing.svelte';
	import Hero from './hero.svelte';
	import Bio from './bio.svelte';
	import Leadership from './leadership.svelte';
	import Experience from './experience.svelte';
	import Skills from './skills.svelte';
	import Languages from './languages.svelte';
	import Contact from './contact.svelte';
</script>

<svelte:head>
	<title>Karni</title>
</svelte:head>

<!-- <Spacing --min="175px" --med="200px" --max="200px" /> -->

<Hero />

<Spacing --min="120px" --med="175px" --max="200px" />

<Bio />

<Spacing --min="120px" --med="175px" --max="200px" />

<Leadership />

<Spacing --min="120px" --med="175px" --max="200px" />

<Experience />

<Spacing --min="120px" --med="175px" --max="200px" />

<Skills />

<Spacing --min="120px" --med="175px" --max="200px" />

<Languages />

<Spacing --min="120px" --med="175px" --max="200px" />

<Contact />

<Spacing --min="75px" --med="100px" --max="120px" />
