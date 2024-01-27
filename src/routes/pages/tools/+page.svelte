<script lang="ts">
import '../../../style.css'
import { Listgroup } from 'flowbite-svelte'

let links = [
    {name: 'VSCode', href: 'https://code.visualstudio.com/'},
    {name: 'git scm', href: 'https://git-scm.com/'},
    {name: 'NodeJS', href: 'https://nodejs.org/en'},
    {name: 'Slack', href: 'https://slack.com/'},
    {name: 'MSTeams', href: 'https://teams.microsoft.com/'},
    {name: 'Jira', href: 'https://www.atlassian.com/software/jira/free'},
    {name: 'GitHub', href: 'https://github.com/'}
]

</script>
<div class="viewport">
    <h2 class="text-2xl font-extrabold dark:text-white">To start we will be working from an online editor</h2>
    <div>
        <a class="font-medium text-blue-800 dark:text-blue-400 hover:underline" rel="stylesheet" href="https://stackblitz.com/?starters=frontend">Stackblitz</a>
        
        <p class="mb-4 text-lg font-normal text-gray-500 dark:text-gray-400">Specifically the HTML/CSS/JS static application</p>
        <img width="500px" alt="Stackblitz" src="/images/tools/stackblitz.jpg">
    </div>
    <br>
    <br>
    <h2 class="text-2xl font-extrabold dark:text-white">Eventually the following tools will need to be installed on your computer</h2>
    <br>
    <div>
        <Listgroup active items={links} let:item class="w-48">
            <a class="text-white" href={item.href} target="_blank">{item.name}</a>
        </Listgroup>
    </div>
</div>