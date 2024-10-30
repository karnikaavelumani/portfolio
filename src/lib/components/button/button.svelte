<!-- src/components/LinkButton.svelte -->
<script lang="ts">
	import { createEventDispatcher } from 'svelte';

	// Define props for the component
	export let link: string = '/'; // Default link
	export let redirect: boolean = false; // Determine if the link opens in a new tab
	export let text: string = 'Submit'; // Default button text
	export let className: string = ''; // Additional CSS class

	const dispatcher = createEventDispatcher();

	// Function to forward the click event
	function forwardClickEvent(ev: MouseEvent) {
		dispatcher('click', ev);
	}
</script>

<!-- Link styled as a button -->
<a
	class="link-button {className}"
	role="button"
	href={link}
	target={redirect ? '_blank' : '_self'}
	rel="noopener noreferrer"
	on:click={forwardClickEvent}
>
	{text}
</a>

<style>
	.link-button {
		display: inline-block; /* Use inline-block to respect button styles */
		text-align: center;
		padding: 12px 24px;
		background-color: none;
		color: black;
		border-radius: 1000px;
		text-decoration: none;
		user-select: none;
		transition: background-color 0.25s ease-in-out;

		&:hover {
			background-color: gray;
		}
	}
</style>
