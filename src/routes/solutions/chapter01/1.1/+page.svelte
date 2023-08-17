<script>
// @ts-nocheck

  import QuestionAns from "../../../../components/QuestionAns.svelte";
</script>

<div class="grid grid-cols-5">
  <div class="col-span-4 px-5 border-x-2 mb-8">
    <h1 class="text-3xl text-slate-500">Solutions for 1.1</h1>
    <div class="mt-5">
      <h1 class="text-2xl">Notes</h1>
      <div class="">
        <blockquote
          class="border-l-2 py-2 pl-3 mt-4 border-slate-700 bg-slate-200"
        >
          Note 1: An algortihm for a computational problem is correct, if for
          all instances of the input if the algorithm <span class="font-bold"
            >halts</span
          >, finishes in finite time, and provides
          <span class="font-bold">correct</span>
          result for all instances of the problem. An incorrect algorithm might not
          stop at all for some input instances or it might halt with incorrect result.
        </blockquote>
      </div>
      <p class="mt-5" />
    </div>
    <QuestionAns navNumber="1.1-1">
      Question: Describe your own real-world example that requires sorting. Describe
      one that requires finding the shortest distance between two points.

      <p slot="answer">
        Real use case of sorting algorithm I encounter daily and use is sorting by date 
        in windows filesystem. It takes a lot of time to sort when there are many files 
        in the folder. Other examples include sorting by price in e-commerce amazon.
        <br/>
        <br/>
        Real life use of shortest path finding algorithm I use often is google maps. I use 
        them often to find shortest path to my destination inside Kathmandu Valley. I am not 
        100% sure of this but shortest path finding algorithms is also used while routing in 
        the internet
      </p>
    </QuestionAns>
    
    <QuestionAns navNumber="1.1-2">
      Question: Other than speed, what other measures of efficiency might
      you need to consider in a real-world setting?

      <p slot="answer">
        How much space (memory) an algorithms take is one of the major thing to
        consider when designing an alorithm. Coding efficiency is also major
        thing to consider (Thanks <a href="https://walkccc.me/CLRS/Chap01/1.1/#11-2">
        walkccc.me</a>).
      </p>
    </QuestionAns>

    <QuestionAns navNumber="1.1-3">
      Question: Select a data structure that you have seen, and discuss its
      strengths and limitations.

      <p slot="answer">
        Array strength will be reading data.
        <br />
        <br />
        But insertion and deletion in middle or beginning of an array can take some
        time because as multiple elements inside the array need to shift their position.
      </p>
    </QuestionAns>
      
    <QuestionAns navNumber="1.1-4">
      Question: How are the shortest-path and traveling-salesperson problems
      given above similar? How are they different?

      <p slot="answer">
        Similarity: Both problems tries to find shortest distance to travel
        <br />
        <br />
        Difference: For travelling salesman we have to travel all the nodes and return
        back to source node but for shortest path finding algorithm we just have
        to find shortest path from start to destination no matter path we take.
      </p>
    </QuestionAns>
    
    <QuestionAns navNumber="1.1-5">
      Question: Suggest a real-world problem in which only the best solution
      will do. Then come up with one in which “approximately” the best
      solution is good enough

      <p slot="answer">
        Best solution: Determining cancerous tumor or a bennign one
        <br />
        <br />
        Approx Best solution: Shortest distance finding on map
      </p>
    </QuestionAns>

    <QuestionAns navNumber="1.1-6">
      Question: Describe a real-world problem in which sometimes the entire
      input is available before you need to solve the problem, but other
      times the input is not entirely available in advance and arrives over
      time.

      <p slot="answer">
        Hit the road jack don't you come back no more no more no more no more
      </p>
    </QuestionAns>
    
  </div>

  <div class="px-2">Navigate Solution</div>
</div>
