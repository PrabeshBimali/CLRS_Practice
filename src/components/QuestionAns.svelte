<script>
// @ts-nocheck
    export let navNumber;

</script>

<div class="mt-9">
    <h1 class="text-2xl">{navNumber}</h1>
    <blockquote class="border-l-2 py-2 pl-3 mt-4 border-slate-700 bg-slate-200">
        <slot/>
    </blockquote>
    
    <p class="mt-5">
      <slot name="answer"/>
    </p>
  </div>