
<script>
	import Clock from '../components/clock.svelte';
	import Score from '../components/score.svelte';
</script>

<div class="background">
    <div class="layout">
        <slot />
    </div>
	<div class="layout">
		<div class="header">
			<Score score={0} />
			<Clock />
		</div>
		<div class="content">
			<slot />
		</div>
	</div>
</div>

<style>
    .background {
        padding: 32px;
	
		padding: 32px;
		display: grid;
		position: absolute;
		inset: 0;
		background-color: var(--color-purple);
	}
	.layout {
		width: 100%;
		max-width: 1024px;
		margin: 0 auto;
		display: grid;
		grid-template-rows: auto 1fr;
		align-items: center;
	}
        position: absolute;
        inset: 0;
	.content,
	.header {
		background-color: white;
		border: 4px solid black;
		padding: 12px 24px;
	}
        background-color: #abacc2;
    }
	.header {
		display: flex;
		justify-content: space-between;
	}
    .layout {
        width: 100%;
        max-width: 900px;
        margin: 0 auto;
    }
</style>
	.content {
		width: 100%;
		max-width: 1024px;
	}





</style>
	import Score from '../components/score.svelte';
</script>

<div class="background">
	<div class="layout">
		<div class="header">
			<Score score={0} />
		</div>
		<div class="content"><slot /></div>
	</div>
</div>



<style>
	.background {
		padding: 32px;
		display: grid;
		position: absolute;
		inset: 0;
		background-color: var(--color-purple);
	}
	.layout {
		width: 100%;
		max-width: 1024px;
		margin: 0 auto;

    display: grid;
		grid-template-rows: auto 1fr;
		align-items: center;
		/* text-align: justify; /* For Edge */
		/* text-align-last: center; */
		/* border: 1px soild rgb(21, 12, 8); */
		/* text-shadow: 0.5px 0.5px #ffffff; */
		/* position: absolute; */
		/* top: 50px; */
	}

.header, 
.content {
  background-color: white;
  border: 4px solid black;
  padding: 12px 24px;

}
.header {
  display: flex;
  justify-content: space-between;
}
</style>
