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


The known parameters that the design is based off of is

<p>S<sub>y</sub> = 36,000 psi</p>
<p>Factor of Safety (FS = 4</p>
<p>P = 800 lbf</p>
<p>&sigma;<sub>allow</sub> = S<sub>y</sub> / FS = 9,000 psi</p>
<p>E = 29,000 psi</p>
<p>&delta;<sub>max</sub> = 0.005 inches</p>

The modulus of elasticity used for calculation (E) is 29,000 psi while the built in modulus of elasticity for the same material in SolidWorks is 29,007,547.53 psi. I updated the elasticity in the parametric equations after noticing this.

Since the inner loop will stay the same, I am adding fixture to the top of the inner loop where the entire design will be hanging off of.

<div style="text-align: center;">
  <img src="A7-3.png" alt="A7-3">
</div>

I will also be adding the applied load to the top of the cylinder holder because this is where the load is originating from. The load will be 800 Lbf because that is was the previously chosen load. This will remain constant for each iteration.

<div style="text-align: center;">
  <img src="A7-4.png" alt="A7-4">
</div>

### Mesh Analysis
For the first test of the each iteration, I used a the medium mesh density with the blended curvature based mesh. For the second test of the each iteration I used the most course blended curvature based mesh. 

For each design iteration, I will check the reliability of the SolidWorks high-quality, curvature-based mesh by conducting a mesh convergence study. The only variable I will change during this study is the mesh density. I will compare a coarse mesh with a medium-density mesh, keeping the mesh type and all other simulation settings the same for each comparison.

I will calculate the percentage change in maximum stress, maximum resultant displacement, and minimum factor of safety using the formula below:

#check to see if formula is working
<p>
  <strong>Change (%) = </strong>
  <span style="display: inline-flex; flex-direction: column; text-align: center; vertical-align: middle;">
    <span style="border-bottom: 1px solid black; padding: 4px 8px;">
      |Medium result − Coarse result|
    </span>
    <span style="padding: 4px 8px;">
      |Coarse result|
    </span>
  </span>
  × 100
</p>


If my FEA results have not converged after three mesh attempts, the assignment allows me to proceed using the results from the finest mesh, documenting that convergence was not achieved.

### Iteration 1

Below is the course mesh

<div style="text-align: center;">
  <img src="A7-5.png" alt="A7-5">
</div>

Below is the FEA simulation for the course mesh

<div style="text-align: center;">
  <img src="A7-6.png" alt="A7-6">
</div>



## Decide



## Communicate

