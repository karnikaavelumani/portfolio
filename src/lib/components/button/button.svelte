<script>
	export let text = 'Click me'; // Default link text
	export let href = '#'; // Default href, pointing to top of the page
	export let disabled = false; // Default disabled state
	export let imageSrc = ''; // Optional image source
	export let imageAlt = ''; // Optional alt text for the image
</script>

<a href={disabled ? undefined : href} class="button {disabled ? 'disabled' : ''}">
	{#if imageSrc}
		<img src={imageSrc} alt={imageAlt} class="button-icon" />
	{/if}
	<span>{text}</span>
</a>

<style>
	.button {
		display: inline-flex;
		align-items: center;
		padding: 3px 10px;
		margin: 5px 0;
		color: black;
		border-radius: 1000px;
		border: 1px solid black;
		text-decoration: none;
		font-size: 14px;
		user-select: none;
		transition: background-color 0.25s ease-in-out;

		&:hover {
			background-color: lightgray;
		}

		&:active {
			background-color: lightblue;
		}
	}

	.button-icon {
		width: 16px; /* Set a size for the icon */
		height: 16px;
		margin-right: 8px; /* Space between icon and text */
	}
</style>
