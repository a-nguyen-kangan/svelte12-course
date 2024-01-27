<script lang="ts">
import '../../../../style.css';
import { Card } from 'flowbite-svelte';
</script>
<br>
<div class="viewport grid grid-cols-1 sm:grid-cols-1 md:grid-cols-3 lg:grid-cols-3 xl:grid-cols-3 gap-10">
      <Card href="https://exercism.org/tracks/javascript/concepts" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          W3Schools JS Quiz
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Attempt the Exercism exercises in the Javascript track.  <br>
          In particular; Basics, Numbers, Arithmetic Operators, Strings, Booleans, Conditionals, Comparison<br>
          Ideally you would have completed everything up to and not including Objects
        </p>
      </Card>

      <Card href="https://www.w3resource.com/javascript-exercises/javascript-basic-exercises.php" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          W3Schools JS Exercises
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Optional:  These are a good bunch of short exercises to practice on!  <br>
          Be aware that sets of exercises can be chosen from the side menu. <br>
        </p>
      </Card>

      <div></div>
      <div></div>
</div>

<style>
    Card {
        display: "inline";
    }
</style>