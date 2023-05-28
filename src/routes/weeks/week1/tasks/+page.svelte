<script lang="ts">
import '../../../../style.css';
import { Card } from 'flowbite-svelte';
</script>
<br>
<div class="viewport grid grid-cols-1 sm:grid-cols-1 md:grid-cols-3 lg:grid-cols-3 xl:grid-cols-4 gap-1">
    <Card href="https://www.freecodecamp.org/learn/2022/responsive-web-design/learn-basic-css-by-building-a-cafe-menu/step-1" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          FreeCodeCamp - Build a Cafe Menu
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Complete the FreeCodeCamp activity to get a basic understanding of HTML and CSS.  Feel free to try some of the other activities in the set!
        </p>
      </Card>

      <Card href="https://www.w3schools.com/quiztest/quiztest.asp?qtest=HTML" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          W3Schools HTML Quiz
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Have a crack at the W3Schools HTML Quiz
        </p>
      </Card>

      <Card href="https://www.w3schools.com/quiztest/quiztest.asp?qtest=CSS" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          W3Schools CSS Quiz
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Have a crack at the W3Schools CSS Quiz
        </p>
      </Card>
      <Card href="https://www.w3resource.com/html-css-exercise/basic/" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          W3Resource: HTML5 Basic (Tag and attribute) - Exercises, Practice, Solution
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Plenty of short exercises to practice on!
        </p>
      </Card>
      <br>
</div>

<style>
    Card {
        display: "inline"
    }
</style>