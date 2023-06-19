<script lang="ts">
  import '../app.postcss';
  import { page } from '$app/stores';
  import { onMount } from 'svelte';
  import {
    Navbar,
    NavBrand,
    NavLi,
    NavUl,
    NavHamburger,
    Sidebar,
    SidebarGroup,
    SidebarItem,
    SidebarWrapper,
    Drawer,
    CloseButton,
    SidebarDropdownWrapper
  } from 'flowbite-svelte';
  import { Cog } from 'svelte-heros-v2';
  import { sineIn } from 'svelte/easing';
  let transitionParams = {
    x: -320,
    duration: 200,
    easing: sineIn
  };
  let breakPoint: number = 1024;
  let width: number;
  let backdrop: boolean = false;
  let activateClickOutside = true;
  let drawerHidden: boolean = false;
  $: if (width >= breakPoint) {
    drawerHidden = false;
    activateClickOutside = false;
  } else {
    drawerHidden = true;
    activateClickOutside = true;
  }
  onMount(() => {
    if (width >= breakPoint) {
      drawerHidden = false;
      activateClickOutside = false;
    } else {
      drawerHidden = true;
      activateClickOutside = true;
    }
  });
  const toggleSide = () => {
    if (width < breakPoint) {
      drawerHidden = !drawerHidden;
    }
  };
  const toggleDrawer = () => {
    drawerHidden = false;
  };
  $: activeUrl = $page.url.pathname;
  let spanClass = 'pl-2 self-center text-md text-gray-900 whitespace-nowrap dark:text-white';
  let divClass = 'w-full md:block md:w-auto pr-8';
  let ulClass = 'flex flex-col p-4 mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-lg md:font-medium';
</script>

<svelte:window bind:innerWidth={width} />
<Navbar let:hidden let:toggle>
  <NavHamburger on:click={toggleDrawer} btnClass="ml-3 lg:hidden" />
  <!-- <NavHamburger on:click={toggle} />
  <NavUl {hidden} {divClass} {ulClass}>
    <NavLi href="/">Home</NavLi>
    <NavLi href="/pages/about">About</NavLi>
    <NavLi href="https://github.com/shinokada/flowbite-sveltekit-responsive-sidebar-layout"
      >GitHub</NavLi
    >
  </NavUl> -->
</Navbar>
<Drawer
  transitionType="fly"
  {backdrop}
  {transitionParams}
  bind:hidden={drawerHidden}
  bind:activateClickOutside
  width="w-64"
  class="overflow-scroll pb-32"
  id="sidebar"
>
  <div class="flex items-center">
    <CloseButton on:click={() => (drawerHidden = true)} class="mb-4 dark:text-white lg:hidden" />
  </div>
  <Sidebar asideClass="w-54">
    <SidebarWrapper divClass="overflow-y-auto py-4 px-3 rounded dark:bg-gray-800">
      <SidebarGroup>
        <SidebarItem label="Home" href="/" on:click={toggleSide} active={activeUrl === `/`} />
        <SidebarItem
          label="About"
          href="/pages/about"
          {spanClass}
          on:click={toggleSide}
          active={activeUrl === '/pages/about'}
        />        
        <SidebarItem
          label="Important tools"
          href="/pages/tools"
          {spanClass}
          on:click={toggleSide}
          active={activeUrl === '/pages/tools'}
        />
        <SidebarDropdownWrapper label="Week 1">
          <SidebarItem
            label="Content - Web"
            href={`/weeks/week1/html`}
            {spanClass}
            on:click={toggleSide}
            active={activeUrl === '/weeks/week1/html'}
          />
          <SidebarItem
          label="Content - Git/GitHub"
          href={`/weeks/week1/git`}
          {spanClass}
          on:click={toggleSide}
          active={activeUrl === '/weeks/week1/git'}
          />
          <SidebarItem
          label="Tasks"
          href={`/weeks/week2/tasks`}
          {spanClass}
          on:click={toggleSide}
          active={activeUrl === '/weeks/week2/tasks'}
          />
        </SidebarDropdownWrapper>
        <SidebarDropdownWrapper label="Week 2">
          <SidebarItem
            label="Content - JavaScript"
            href={`/weeks/week2/javascript`}
            {spanClass}
            on:click={toggleSide}
            active={activeUrl === '/weeks/week2/javascript'}
          />
          <SidebarItem
          label="Tasks"
          href={`/weeks/week2/tasks`}
          {spanClass}
          on:click={toggleSide}
          active={activeUrl === '/weeks/week2/tasks'}
          />
        </SidebarDropdownWrapper>
        <SidebarDropdownWrapper label="Week 3">
          <SidebarItem
            label="Content - JavaScript Functions"
            href={`/weeks/week3/javascript_functions`}
            {spanClass}
            on:click={toggleSide}
            active={activeUrl === '/weeks/week3/javascript_functions'}
          />
          <SidebarItem
          label="Content - JavaScript Arrays"
          href={`/weeks/week3/javascript_arrays`}
          {spanClass}
          on:click={toggleSide}
          active={activeUrl === '/weeks/week3/javascript_arrays'}
        />
        </SidebarDropdownWrapper>
      </SidebarGroup>
    </SidebarWrapper>
  </Sidebar>
</Drawer>
<div class="flex px-4 mx-auto w-full dark:bg-gray-800">
  <main class="lg:ml-72 w-full mx-auto">
    <slot />
  </main>
</div>