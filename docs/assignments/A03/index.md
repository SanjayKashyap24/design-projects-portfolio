# A3 – Parametric and FEA

## Objective
The purpose of this assignment is to parametrically design a bar with a circular cross section that is subjected to an axial load between 300 lbf and 500 lbf such that the bar's maximum axial deflection does not exceed 0.009 inches. The bar is to be designed from aluminum with a Young's modulus in the range of 8.5–11.5 × 10⁶ psi. Then we are supposed to run an FEA simulation on the CAD model we created and afterwards reflect on the differences between the calculations used to design the model and what the FEA simulation shows.

## Analyze
### Initial Decisions
I chose to use an initial diameter of 1 inch and an elasticity of 8.5 × 10⁶ psi. I wanted to design a bar that bends more easily and I thought that a bar that bends easily would need a girthy diameter. My next step was to set up the global variables on SolidWorks (my CAD software of choice) to keep track of my variables.

<div style="text-align: center;">
  <img src="GlobaVariables1.png" alt="Initial dimensions chart">
</div>

### Setting Up Equations

I used the stress and strain equations and Hook's Law to algebraically solve for the variable length.   

<p align="center"><strong>Stress</strong></p>
<p align="center"><strong>σ = F/A</strong></p>

<p><strong>F</strong> = Applied Axial Force</p>
<p><strong>A</strong> = Cross-sectional area</p>
<p><strong>σ</strong> = stress</p>

<p align="center"><strong>Strain</strong></p>
<p align="center"><strong>ε = δ/L</strong></p>

<p><strong>L</strong> = Length</p>
<p><strong>δ</strong> = Deflection</p>
<p><strong>ε</strong> = Strain</p>

<p align="center"><strong>Hooke's Law</strong></p>
<p align="center"><strong>σ = Eε</strong></p>

<p><strong>E</strong> = Young's modulus of elasticity</p>

<p align="center"><strong>Algebra</strong></p>

<p>Insert the stress and strain equations into Hooke's Law</p>

<p align="center">F/A = E(δ/L)</p>

<div align="center">
<table style="border: 4px solid black;" cellpadding="10"><tr><td><strong>δ = FL/(AE)</strong></td></tr></table>
</div>


## Decide


## Communicate

