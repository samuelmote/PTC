<script>
    export let answer= true;
 </script>
 {#if answer}
 <p style="color: green; "> Great job</p>
    {:else} 
    <p style="color: red;"> wasn't quite right...</p>
 {/if}