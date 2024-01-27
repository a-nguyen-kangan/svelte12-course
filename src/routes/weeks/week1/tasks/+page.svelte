<script lang="ts">
import '../../../../style.css';
import { Card } from 'flowbite-svelte';
</script>
<br>
<h2 class="text-2xl font-extrabold dark:text-white p-5">Week 1 - Tasks</h2>
<h2 class="text-2xl font-extrabold dark:text-white p-5">Day 1: HTML</h2>
<div class="viewport grid grid-cols-1 sm:grid-cols-1 md:grid-cols-3 lg:grid-cols-3 xl:grid-cols-3 gap-10">
    <!-- <Card href="https://www.freecodecamp.org/learn/2022/responsive-web-design/learn-basic-css-by-building-a-cafe-menu/step-1" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          FreeCodeCamp - Build a Cafe Menu
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Complete the FreeCodeCamp activity to get a basic understanding of HTML and CSS.  Feel free to try some of the other activities in the set!
        </p>
      </Card> -->
      <Card img = "/images/week1/catphotoapp.jpg" href="https://www.freecodecamp.org/learn/2022/responsive-web-design/learn-html-by-building-a-cat-photo-app/step-1" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          FreeCodeCamp - Building a cat photo app
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Complete the FreeCodeCamp activity to get a basic understanding of HTML.  Feel free to try some of the other activities in the set!
          This can be done either on the FreeCodeCamp site or on StackBlitz
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

 
      <div></div>
      <div></div>
      <!-- <Card href="https://www.w3resource.com/html-css-exercise/basic/" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          W3Resource: HTML5 Basic (Tag and attribute) - Exercises, Practice, Solution
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Plenty of short exercises to practice on!
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
      <Card img="/images/week1/todo_basic.jpg" href="https://lively-pony-d1285d.netlify.app/" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Week 1 Task</h5>
        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Have a look and play at the linked site and try to re-create the look using HTML and CSS
        </p>
      </Card> -->
</div>
<h2 class="text-2xl font-extrabold dark:text-white p-5">Day 2: CSS</h2>
<div class="viewport grid grid-cols-1 sm:grid-cols-1 md:grid-cols-3 lg:grid-cols-3 xl:grid-cols-3 gap-10">
  <Card img="/images/week1/htmltodo.jpg" href="/images/week1/htmltodo.jpg" target="_blank">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
      HTML consolidation task: HTML only Todo list
    </h5>
    <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
      Build a simple todo list using HTML only.  
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
  <Card img="/images/week1/omelettestyled.jpg" href="/resources/omelette.html" target="_blank">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
      CSS Task: Style a recipe
    </h5>
    <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
      Style the provided HTML using css
      exercise c/o frontendmentor.io
      <br>
      <br>
      Use the "view page source" tool to get the HTML and image
    </p>
  </Card>

  <div></div>
</div>

<style>
    Card {
        display: "inline";
    }
</style>