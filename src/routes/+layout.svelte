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
        
		background-color: #e3a68d;
	}
    .layout {
        width: 100%;
        max-width: 524px;
        margin: 50 auto;
		text-align: justify; /* For Edge */
  text-align-last: center;
		border:1px soild rgb(21, 12, 8);
  text-shadow: .5px .5px #ffffff;
  position: absolute;
  top: 50px;
  border: 7px solid rgb(0, 0, 0);


}
.layout {
  position: absolute;
  left: 460px;
  top: 100px;
}
</style>
 
need to find out how to make font/text bigger