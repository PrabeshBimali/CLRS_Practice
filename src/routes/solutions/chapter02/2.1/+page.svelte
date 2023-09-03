<script>
  import Heading from "../../../../components/Heading.svelte";
  import Note from "../../../../components/Note.svelte";
  import QuestionAns from "../../../../components/QuestionAns.svelte";
</script>

<div class="grid grid-cols-5">
  <div class="col-span-4 px-5 border-x-2 mb-8">
    <Heading>2.1 Insertion sort</Heading>

    <Note>
      Note1: When we sort something usually we take a single column from a record
      and sort according to the column, this column we choose is also known as key. 
      For example, lets say we have a database with columns (course name, credits, 
      Date etc.). Now from this course database we can choose to sort the records 
      based on credits, which will be key, and next time we can choose date so date 
      will be key and records will be sorted based on it.
    </Note>
    <QuestionAns navNumber="2.1-1">
      This is Q

      <p slot="answer">
        Answer
      </p>
    </QuestionAns>
    
  </div>
</div>
