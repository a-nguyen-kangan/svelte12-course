<script lang="ts">
import '../../../../style.css';
import { Card } from 'flowbite-svelte';
</script>
<br>
<div class="viewport grid grid-cols-1 sm:grid-cols-1 md:grid-cols-3 lg:grid-cols-3 xl:grid-cols-3 gap-10">
      <Card href="https://www.w3schools.com/js/js_quiz.asp" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          W3Schools JS Quiz
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Have a crack at the W3Schools HTML Quiz
        </p>
      </Card>

      <Card href="https://www.w3resource.com/javascript-exercises/javascript-basic-exercises.php" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          W3Schools JS Exercises
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          These are a good bunch of short exercises to practice on!  <br>
          Be aware that sets of exercises can be chosen from the side menu. <br>
          The JS HTML DOM set of exercises are essential to do.
        </p>
      </Card>
      <Card href="https://www.w3resource.com/javascript-exercises/javascript-dom-exercises.php" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          W3Resource: JavaScript (HTML DOM) - Exercises, Practice, Solution
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Short tasks/exercises to practice DOM manipulation
        </p>
      </Card>
      <Card img="/images/week1/todo_basic.jpg" href="https://lively-pony-d1285d.netlify.app/" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Week 1 Task</h5>
        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight"></p>
          Try to recreate:
          <ul class="max-w-md space-y-1 text-gray-500 list-disc list-inside dark:text-gray-400"> 
            <li>alert when the add button is clicked</li>
            <li>add a new item to "Item to Add:" text</li>
            <li>remove text from "Item to Add:" on clicking "Remove Item to Add"</li>
            <li>Create the "Set Heading to Red" button and functionality</li>
        </ul>

      </Card>
</div>

<style>
    Card {
        display: "inline";
    }
</style>