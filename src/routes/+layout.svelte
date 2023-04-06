<div class="background">
	<div class="layout">
		<slot />
	</div>
</div>

<style>
	.background {
        padding: 32px;
		position: absolute;
		inset: 0;
        
		background-color: #378590;
	}
    .layout {
        width: 100%;
        max-width: 1024px;
        margin: o auto;
    }
</style>
