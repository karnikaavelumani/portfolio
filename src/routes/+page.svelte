<script>
	import Spacing from '$lib/spacing.svelte';
	import Page1 from './page1.svelte';
	import Page2 from './page2.svelte';
	import Page3 from './page3.svelte';
</script>

<svelte:head>
	<title>Karni</title>
</svelte:head>

<Page1 />

<Spacing --min="75px" --med="100px" --max="30px" />

<Page2 />

<Spacing --min="75px" --med="100px" --max="120px" />

<Page3 />

<Spacing --min="75px" --med="100px" --max="120px" />
