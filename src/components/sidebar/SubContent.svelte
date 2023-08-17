<script>
// @ts-nocheck
    let toggleSubContent = -1; 
    export let subcontent;

    function handleToggle() {
        if(toggleSubContent === 1){
            toggleSubContent = -1;
        }
        else {
            toggleSubContent = 1;
        }
        

    }

</script>

<!-- svelte-ignore a11y-click-events-have-key-events -->
<!-- svelte-ignore a11y-no-noninteractive-element-interactions -->
<nav class="cursor-pointer flex flex-col gap-2">
  <!-- svelte-ignore a11y-no-static-element-interactions -->
  <span on:click={handleToggle} class="hover:text-sky-700">{subcontent.name}</span>
  {#if toggleSubContent > 0}
    {#each subcontent.content as content}
        <nav class="pl-3">
            <a class="hover:text-sky-700" href={content.href}>{content.name}</a>
        </nav>
    {/each}
  {/if}
</nav>
