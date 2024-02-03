<script lang="ts">
import '../../../../style.css';
import { Card } from 'flowbite-svelte';
</script>
<br>
<h2 class="text-2xl font-extrabold dark:text-white p-5">Week 2 - Tasks</h2>
<h2 class="text-2xl font-extrabold dark:text-white p-5">Day 1: Selectors and Flexbox</h2>
<div class="grid grid-cols-1 sm:grid-cols-1 md:grid-cols-3 lg:grid-cols-3 xl:grid-cols-3 gap-10">
  <Card href="https://codepen.io/Colt/pen/rNrrBoW" target="_blank">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
      CSS Selectors Exercise
    </h5>
    <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
      Practice your CSS selectors with this exercise on CodePen!
      <br>
      Only change the CSS, not the HTML!
    </p>
  </Card>

  <Card img="/images/week2/flexboxfroggy.jpg" href="https://flexboxfroggy.com/" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          Flexbox Froggy
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Try the Flexbox Froggy game to get a better understanding of Flexbox.  You should be able to do everything up to exercise 23.  24 can be a little tricky, but give it a go!
        </p>
      </Card>

      
      <!-- <Card href="https://www.w3resource.com/javascript-exercises/javascript-dom-exercises.php" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          Todo List App
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Update the Todo List App from week 1 to incorporate some styling.<br>
          You can use the design from the week 1 task as a starting point.
        </p>
      </Card> -->
      <Card img="/images/week2/flexpractice.png">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
          Layout Practice with Flexbox
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          See if you can put what you've learnt into practice by attempting to replicate this layout, taken from The Odin Project.
        </p>
      </Card>
      <Card img="/images/week2/flexpracticestyles.png">
        
        <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
          Some styling which you may choose to follow.
        </p>
      </Card>
      <!-- <Card img="/images/week1/todo_basic.jpg" href="https://lively-pony-d1285d.netlify.app/" target="_blank">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Week 1 Task</h5>
        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight"></p>
          Try to recreate:
          <ul class="max-w-md space-y-1 text-gray-500 list-disc list-inside dark:text-gray-400"> 
            <li>alert when the add button is clicked</li>
            <li>add a new item to "Item to Add:" text</li>
            <li>remove text from "Item to Add:" on clicking "Remove Item to Add"</li>
            <li>Create the "Set Heading to Red" button and functionality</li>
        </ul>

      </Card> -->

</div>
<h2 class="text-2xl font-extrabold dark:text-white p-5">Day 2: CSS libraries & Forms</h2>
<div class="viewport grid grid-cols-1 sm:grid-cols-1 md:grid-cols-3 lg:grid-cols-3 xl:grid-cols-3 gap-10">
  <Card img="/images/week2/speakersubmission.png">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
      Recreate a form which contains various user input fields
    </h5>
    <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
      Firstly, set up the html skeleton for the form and check if the data is being sent correctly to https://jsonplaceholder.typicode.com/posts
    </p>
    <p class="font-normal text-gray-700 dark:text-gray-400 leading-tight">
      After that, attempt to style the page via CSS. Or for the adventurous, incorporate a CSS library.
    </p>
  </Card>


</div>

<style>
    Card {
        display: "inline";
    }
</style>