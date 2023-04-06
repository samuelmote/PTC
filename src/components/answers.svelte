<script>
	export let answer = true;
</script>

{#if answer}
	<p class="correct">Great Job, That's Right...</p>
{:else}
	<p class="incorrect">Isn't Quite Right...</p>
{/if}

<style>
	.correct {
		color: green;
		font-weight: bold;
		text-decoration: underline;
	}
	.incorrect {
		color: red;
		font-weight: bold;
		text-decoration: underline;
	}
</style>
