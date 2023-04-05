<script>
    export let answer= true;
 </script>
 {#if answer}
 <p style="color: green; "> Great Job, That's Right...</p>
    {:else} 
    <p style="color: red;"> Isn't Quite Right...</p>
 {/if}