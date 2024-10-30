<script>
	import Spacing from '$lib/spacing.svelte';
	import Hero from './hero.svelte';
	import About from './about.svelte';
	import Experience from './exp.svelte';
</script>

<svelte:head>
	<title>Karni's Portfolio</title>
</svelte:head>

<Hero />
<About />
<Experience />

<Spacing --min="75px" --med="100px" --max="30px" />
