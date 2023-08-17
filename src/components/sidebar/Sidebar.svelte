<script>
  // @ts-nocheck

  import SubContent from "./SubContent.svelte";
  import { mainContents, subContents } from "./contentsData";

  let toggleSubHeadings = -1;

  function handleToggle(chapter) {
    if (toggleSubHeadings === chapter) {
      toggleSubHeadings = -1;
    } else {
      toggleSubHeadings = chapter;
    }
    console.log(chapter);
  }
</script>

<nav class="p-5 flex flex-col gap-3 text-sm">
  {#each mainContents as content}
    <div class="list-none">
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <!-- svelte-ignore a11y-no-static-element-interactions -->
      <span 
        class="{toggleSubHeadings === content.chapter
          ? 'text-green-700'
          : 'text-black'} cursor-pointer hover:text-sky-700"
        on:click={() => handleToggle(content.chapter)}>{content.name}</span
      >
      <nav class="flex flex-col pl-3 gap-2">
      {#if toggleSubHeadings == 0 && content.chapter == toggleSubHeadings}
        {#each subContents[toggleSubHeadings] as subcontent}
          <SubContent subcontent={subcontent}/>
        {/each}
      {/if}
      </nav>
    </div>
  {/each}
</nav>
