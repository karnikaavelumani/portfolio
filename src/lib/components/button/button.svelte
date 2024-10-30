<script>
	export let text = 'Click me'; // Default link text
	export let href = '#'; // Default href, pointing to top of the page
	export let disabled = false; // Default disabled state
</script>

<a href={disabled ? undefined : href} class="button {disabled ? 'disabled' : ''}">
	{text}
</a>

<style>
	.button {
		display: inline-block;
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

		/* on click */
		&:active {
			background-color: lightblue;
		}
	}
</style>
