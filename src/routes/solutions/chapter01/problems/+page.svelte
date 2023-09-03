<script>
  import QuestionAns from "../../../../components/QuestionAns.svelte";
  import MathInline from "../../../../components/MathInline.svelte";
  import Heading from "../../../../components/Heading.svelte";
</script>

<Heading>Chapter 1 Problems</Heading>
<QuestionAns navNumber="1-1">
  For each function f (n) and time t in the following table, determine the
  largest size n of a problem that can be solved in time t, assuming that the
  algorithm to solve the problem takes f (n) microseconds.

  <div slot="answer" class="relative overflow-x-auto">
    <table class="w-full text-sm text-left text-gray-500">
      <thead class="text-xs text-gray-700 uppercase bg-gray-50">
        <tr>
          <th scope="col" class="px-3 py-3">f(n)</th>
          <th scope="col" class="px-3 py-3">1 second</th>
          <th scope="col" class="px-3 py-3">1 minute</th>
          <th scope="col" class="px-3 py-3">1 hour</th>
          <th scope="col" class="px-3 py-3">1 day</th>
          <th scope="col" class="px-3 py-3">1 month</th>
          <th scope="col" class="px-3 py-3">1 year</th>
          <th scope="col" class="px-3 py-3">1 century</th>
        </tr>
      </thead>
      <tbody>
        <tr class="bg-white border-b">
          <th
            scope="row"
            class="px-3 py-4 font-medium text-gray-900 whitespace-nowrap"
          >
            <MathInline>log(n)</MathInline>
          </th>
          <td class="px-3 py-4 text-center">
            <MathInline>{`2^{10^6}`}</MathInline>
          </td>
          <td class="px-3 py-4 text-center">
            <MathInline>{`2^{6*10^7}`}</MathInline>
          </td>
          <td class="px-3 py-4 text-center">
            <MathInline>{`2^{3.6*10^9}`}</MathInline>
          </td>
          <td class="px-3 py-4 text-center">
            <MathInline>{`2^{8.64*10^{10}}`}</MathInline>
          </td>
          <td class="px-3 py-4 text-center">
            <MathInline>{`2^{2.59*10^{12}}`}</MathInline>
          </td>
          <td class="px-3 py-4 text-center">
            <MathInline>{`2^{3.11*10^{13}}`}</MathInline>
          </td>
          <td class="px-3 py-4 text-center">
            <MathInline>{`2^{3.11*10^{15}}`}</MathInline>
          </td>
        </tr>
        <tr class="bg-white">
          <th
            scope="row"
            class="px-3 py-4 font-medium text-gray-900 whitespace-nowrap"
          >
            <MathInline>\sqrt n</MathInline>
          </th>
          <td class="px-3 py-4 text-center">
            <MathInline>{`10^{12}`}</MathInline>
          </td>
          <td class="px-3 py-4 text-center">
            <MathInline>{`3.6*10^{15}`}</MathInline>
          </td>
          <td class="px-3 py-4 text-center">
            <MathInline>{`1.3*10^{19}`}</MathInline>
          </td>
          <td class="px-3 py-4 text-center">
            <MathInline>{`7.46*10^{21}`}</MathInline>
          </td>
          <td class="px-3 py-4 text-center">
            <MathInline>{`6.71*10^{24}`}</MathInline>
          </td>
        </tr>
        <tr class="bg-white">
          <th
            scope="row"
            class="px-3 py-4 font-medium text-gray-900 whitespace-nowrap"
          >
            <MathInline>n</MathInline>
          </th>
          <td class="px-3 py-4 text-center">
            <MathInline />
          </td>
        </tr>
        <tr class="bg-white">
          <th
            scope="row"
            class="px-3 py-4 font-medium text-gray-900 whitespace-nowrap"
          >
            <MathInline>nlog(n)</MathInline>
          </th>
          <td class="px-3 py-4 text-center">
            <MathInline>2^n</MathInline>
          </td>
        </tr>
        <tr class="bg-white">
          <th
            scope="row"
            class="px-3 py-4 font-medium text-gray-900 whitespace-nowrap"
          >
            <MathInline>n^2</MathInline>
          </th>
          <td class="px-3 py-4 text-center">
            <MathInline>2^n</MathInline>
          </td>
        </tr>
        <tr class="bg-white">
          <th
            scope="row"
            class="px-3 py-4 font-medium text-gray-900 whitespace-nowrap"
          >
            <MathInline>n^3</MathInline>
          </th>
          <td class="px-3 py-4 text-center">
            <MathInline>2^n</MathInline>
          </td>
        </tr>
        <tr class="bg-white">
          <th
            scope="row"
            class="px-3 py-4 font-medium text-gray-900 whitespace-nowrap"
          >
            <MathInline>2^n</MathInline>
          </th>
          <td class="px-3 py-4 text-center">
            <MathInline>2^n</MathInline>
          </td>
        </tr>
        <tr class="bg-white">
          <th
            scope="row"
            class="px-3 py-4 font-medium text-gray-900 whitespace-nowrap"
          >
            <MathInline>n!</MathInline>
          </th>
          <td class="px-3 py-4 text-center">
            <MathInline>2^n</MathInline>
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</QuestionAns>
