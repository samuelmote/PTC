<script>
    export let answer= true;
 </script>
 {#if answer}
 <p>Great job</p>
    {:else} 
    <p> wasn't quite right...</p>
 {/if}