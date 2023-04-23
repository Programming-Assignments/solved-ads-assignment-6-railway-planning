Download Link: https://assignmentchef.com/product/solved-ads-assignment-6-railway-planning
<br>
The railway system was heavily oversized during the end of the Cold War and the party secretary from Minsk has been tasked with liquidate money from the budget by removing some routes. Still the minister of transport demands that it should be possible to transport <em>C </em>people a day from Minsk to Lund, since that is the number of students that want to take part in the incredible course in Algorithms.

Luckily, as help, you have a map over all routes. Furthermore you have constructed a list over the routes that would be most profitable to remove.

<h1>Aims</h1>

The goals of the lab are:

<ul>

 <li>Implementing a Network-Flow-algorithm.</li>

 <li>Debugging your code.</li>

 <li>Structuring your code in a logical fashion.</li>

 <li>Reason about correctness of your algorithm.</li>

 <li>Reason about upper bounds for time complexity.</li>

</ul>

<h1>Problem formulation</h1>

You are given the structure of the railway system, in the form of nodes (cities) and edges (routes connecting the cities). For each edge you will be given the capacity (the number of students it can carry). Then you will be given a plan for which routes to remove in a specific order – in which you need to remove the routes if possible. If you cannot (which you cannot if the total maximal flow from the Minsk to Lund is less than <em>C</em>) remove a route you stop your plan and instead you start implementing the plan. Your task is to answer how many of the routes on your list you can remove and what the maximal flow of students from Minsk to Lund will be after removing these routes.

<h1>Input</h1>

The first line consists of four integers <em>N,M,C,P</em>, the number of nodes, the number of edges, the number of students to transfer from Minsk (node 0) to Lund (node <em>N </em>−1) and the number of routes in your plan. It is guaranteed that  and that the capacity of the network before any routes are

removed is at least <em>C</em>. Then follows <em>M </em>lines where the <em>i</em>-th line (0-indexed) consists of three integers <em>u<sub>i</sub>,v<sub>i</sub>,c<sub>i</sub></em>, where 0≤ <em>u<sub>i</sub>,v<sub>i </sub>&lt; N </em>are the nodes and <em>c<sub>i </sub></em>is the capacity of the route, 1≤ <em>c<sub>i </sub></em>≤100. Note that students can travel both from <em>u<sub>i </sub></em>to <em>v<sub>i </sub></em>and from <em>v<sub>i </sub></em>to <em>u<sub>i </sub></em>(the graph is undirected) but in total at most <em>c<sub>i </sub></em>soldiers. It is guaranteed that the each pair of nodes occurs at most once in the input and that <em>u<sub>i </sub></em>6= <em>v<sub>i</sub></em>. Then follows <em>P </em>lines with one integer each, where the <em>i</em>-th line contains the index of the <em>i</em>-th route you want to remove. Note that you have to remove them in exactly this order as they are given and it is guaranteed that all routes you want to remove are unique in the input.

<h1>Output</h1>

The output should contain one line with two space-separated integers <em>x,f</em>, where <em>x </em>is the number of routes you can remove (while still having a maximal flow of at least <em>C</em>) and <em>f </em>is the maximal flow from node 0 to node <em>N </em>−1 after removing these routes.

<h1>Examination and Points of Discussion</h1>

To pass the lab make sure you have:

<ul>

 <li>Have successfully implemented the algorithm with the correct time complexity.</li>

 <li>Have neat and understandable code.</li>

 <li>Have descriptive variable names.</li>

 <li>Have filled in the blanks in the report.</li>

 <li>Have run the check_solution script to validate your solution.</li>

</ul>

During the oral presentation you will discuss the follwoing questions with the lab assistant:

<ul>

 <li>What is the time complexity, and more importantly why?</li>

 <li>Which other (well-known) algorithmic problems can be solved using Network-Flow?</li>

 <li>If the capacities of the edges are very large, how can one get a different (better) time complexity?</li>

</ul>

<strong>Sample Input 1                                                                                 Sample Output 1</strong>

<table width="622">

 <tbody>

  <tr>

   <td width="311">3 3 10 30 1 100     2 101     2 10021</td>

   <td width="311">2 10</td>

  </tr>

 </tbody>

</table>


