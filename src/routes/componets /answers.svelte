<script>
    export let answer = false;
 </script>
 {#if answer}
 <p>
    Great job - that was the answer!
 </p>
 {/if}
 <script>
    export let answer = true;
 </script>
 {#if answer}
 <p>
    Oh man, that answer wasn't quite right...
 </p>
 {/if}