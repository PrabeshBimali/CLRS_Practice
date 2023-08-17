<script>
  import QuestionAns from "../../../../components/QuestionAns.svelte";
  import MathInline from "../../../../components/MathInline.svelte";
  import MathBlock from "../../../../components/MathBlock.svelte";

</script>
<div class="grid grid-cols-5">
    <div class="col-span-4 px-5 border-x-2 mb-8">
      <h1 class="text-3xl text-slate-500">1.2 Algorithm as a Technology</h1>
      <div class="mt-5">
        <h1 class="text-2xl">Notes</h1>
        <div class="">
          <blockquote class="border-l-2 py-2 pl-3 mt-4 border-slate-700 bg-slate-200">
            Note 1: If computers were infinitely fast and infinite storage we still need to 
            study algorithms as it still has to produce correct result and terminate. Although 
            easiest algorithm will do, if that were the case. Time and memory are not infinite 
            in computer so we should choose algorithms that use time and space efficiently.
          </blockquote>
        </div>
        <p class="mt-5" />
      </div>

      <QuestionAns navNumber="1.2-1">
        Question: Give an example of an application that requires algorithmic content at
        he application level, and discuss the function of the algorithms involved

        <p slot="answer">
          Almost all big software use algorithms for different funtionalities. Youtube uses
          search algorithm when searching for videos. Recommendation system designed to put 
          engaging content based on user's behaviour in recommended tab. Proabably, some sorting 
          algorithm for sorting videos or comments from newest to oldest.
        </p>
      </QuestionAns>
      
      <QuestionAns navNumber="1.2-2">
        Question: Suppose that for inputs of size n on a particular computer, insertion sort
        runs in <MathInline>8n^2</MathInline> steps and merge sort runs in <MathInline>64nlog(n)
        </MathInline> steps. For which values of n does insertion sort beat merge sort?

        <p slot="answer">
            <MathBlock>{`8n^2 < 64nlog(n)`}</MathBlock>
            <MathBlock>{`n/8 < log(n)`}</MathBlock>
            <MathBlock>{`2^{n/8} < n`}</MathBlock>
        </p>
      </QuestionAns>
      <QuestionAns navNumber="1.2-3">
        What is the smallest value of n such that an algorithm whose running time is 
        <MathInline>100n^2</MathInline> runs faster than an algorithm whose running time is 
        <MathInline>2^n</MathInline> on the same machine?

        <p slot="answer">
          When n = 14, <MathInline>100n^2</MathInline> = 19,600 and <MathInline>2^n</MathInline> = 16,384
          <MathBlock>{`100n^2 > 2^n`}</MathBlock>
          When n = 15, <MathInline>100n^2</MathInline> = 22,500 and <MathInline>2^n</MathInline> = 32,768
          <MathBlock>{`100n^2 < 2^n`}</MathBlock>
          So, For <MathInline>n \ge 15</MathInline> running time of <MathInline>{`100n^2 < 2^n`}</MathInline>
        </p>
      </QuestionAns>
    </div>
    <div class="px-2">Navigate Solution</div>
  </div>
  