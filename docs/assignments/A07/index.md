# A7 – FEA on a Bracke

## Objective
Your task is simply to create a high stiff, high strength, and lightweight component. Use Finite Element analysis to drive your decision making process throughout your design. Each step of the analysis and before you make geometric changes make sure the component’s results (stress/displacement/Safety Factor) converge on a 7% difference. Achieve this by modifying the number of elements. If after three attempts to converge use the stiffness and stress from the finer mesh size use the finest mesh size and proceed through the process.


* Use Finite Element Analysis (FEA) to improve the bracket design from previous assignments.
* Ensure high stiffness, strength, and lightweight optimization through iterative design.
* Conduct multiple FEA simulations, refining geometry based on results.
* Perform static stress analysis, including constraints, loading, and meshing selection.
* Interpret data by identifying max stress, displacement, and safety factors.
* Optimize the design by modifying geometry to enhance performance.
* Document the entire process with images, calculations, and insights.
* Reflect on key engineering lessons learned and time spent.

## Analyze
The workflow for the component design has an outer loop and an inner loop. The inner loop’s function  is to validate the results. The outer loop’s function is for the geometry design optimization.

When initially designing my part I used steel (ASTM A36) because the properties are already in SolidWorks and cost is not a constraint. I will continue to use this material for my further analysis.

<div style="text-align: center;">
  <img src="A7-1.png" alt="A7-1">
</div>

<div style="text-align: center;">
  <img src="A7-2.png" alt="A7-2">
</div>

I will be evaluating each iteration of my design with the table below where the first iteration is the original design A5 and A6 assignment.


<style>
    .design-table {
        width: 100%;
        border-collapse: collapse;
        table-layout: fixed;
        font-family: "Times New Roman", serif;
        font-size: 20px;
        color: black;
    }

    .design-table th,
    .design-table td {
        border: 2px solid black;
        padding: 10px;
        text-align: left;
        vertical-align: middle;
    }

    .design-table th {
        font-weight: bold;
    }

    .design-table th:first-child,
    .design-table td:first-child {
        width: 25%;
    }

    .design-table td {
        height: 24px;
    }
</style>

<table class="design-table">
    <thead>
        <tr>
            <th></th>
            <th>Design 1</th>
            <th>Design II</th>
            <th>Design III</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Max Stress and location</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Max deflection and<br>location</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>mass</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Safety Factor</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Number of elements</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>

Since the inner loop will stay the same, I am adding fixture to the top of the inner loop where the entire design will be hanging off of.

<div style="text-align: center;">
  <img src="A7-3.png" alt="A7-3">
</div>

I will also be adding the applied load to the top of the cylinder holder because this is where the load is originating from.

<div style="text-align: center;">
  <img src="A7-4.png" alt="A7-4">
</div>

### Design 1


## Decide


## Communicate

