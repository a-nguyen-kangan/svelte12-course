<script lang="ts">
import '../../../style.css'
import { Listgroup } from 'flowbite-svelte'

let links = [
    {name: 'VSCode', href: 'https://code.visualstudio.com/'},
    {name: 'git scm', href: 'https://git-scm.com/'},
    {name: 'NodeJS', href: 'https://nodejs.org/en'},
    {name: 'Slack', href: 'https://slack.com/'},
    {name: 'MSTeams', href: 'https://teams.microsoft.com/'}
]

</script>
<div class="viewport">
    <h2 class="text-4xl font-extrabold dark:text-white">The following tools will need to be installed on your computer</h2>
    <br>
    <div>
        <Listgroup active items={links} let:item class="w-48">
            <a href={item.href} target="_blank">{item.name}</a>
        </Listgroup>
    </div>
</div>