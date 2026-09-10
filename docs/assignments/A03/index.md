# A3 – Parametric Modeling and FEA

## Objective
The purpose of this assignment is to parametrically design a bar with a circular cross section that is subjected to an axial load between 300 lbf and 500 lbf such that the bar's maximum axial deflection does not exceed 0.009 inches. The bar is to be designed from aluminum with a Young's modulus in the range of 8.5–11.5 × 10⁶ psi. Then we are supposed to run an FEA simulation on the CAD model we created and afterwards reflect on the differences between the calculations used to design the model and what the FEA simulation shows.

## Analyze

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
<table border="3" cellpadding="10"><tr><td><strong>δ = FL/(AE)</strong></td></tr></table>
</div>

## Modeling

### Creating the CAD Model
I chose to use an initial diameter of 1 inch and an elasticity of 10 × 10⁶ psi. I wanted to design a bar that bends more easily and I thought that a bar that bends easily would need a wide diameter. My next step was to set up the global variables on SolidWorks (my CAD software of choice) to automatically define the measurements I have calculated.

<div style="text-align: center;">
  <img src="GlobaVariables1.png" alt="Initial dimensions chart">
</div>

Below is a picture of the finished model before I begin the FEA.

<div style="text-align: center;">
  <img src="BarPic1.png" alt="BarPic1">
</div>


### FEA
When choosing the parameters for the FEA simulation, I chose to create the bar out of 6061-T6 (SS) aluminum because it had the closest modulus of elasticity to the one I chose when designing the bar. Then I chose which side of the bar would be fixed to the wall and which side would be loaded.

<div style="text-align: center;">
  <img src="ChosenMaterial.png" alt="MaterialSelection">
</div>

<div style="text-align: center;">
  <img src="FixedBar.png" alt="FixedPoint">
</div>

<div style="text-align: center;">
  <img src="LoadedBar.png" alt="LoadedPoint">
</div>

Next I added a mesh and I chose the option closest to the middle between gritty and fine. The Mesh breaks the surfaces into smaller parts for the FEA simulation to analyze.

<div style="text-align: center;">
  <img src="MeshBar.png" alt="Mesh">
</div>

The next step was to run the FEA and analyze the resulting Von Mises stress map to ensure that the maximum stress on the bar does not exceed the strength of the aluminum.

<div style="text-align: center;">
  <img src="ActualBarStress.png" alt="Stress">
</div>

The Von Mises stress map showed the maximum stress was 0.07445 psi, which was lower than the yield strength of the aluminum was 39890 psi concluding the project with a factor of safety of 53.6 (factor of safety calculation below).


<div align="center">
Factor of Safety <strong>=</strong> Yield Strength &divide; Max Stress <strong>=</strong> 39890 psi &divide; 744.4 psi <strong>=</strong> <strong>53.6</strong>
</div>


Below is the simulated deflection.

<div style="text-align: center;">
  <img src="BarStress.png" alt="Deflection">
</div>

## Reflection
There was a significant difference between the maximum deflection within the simulation and what I believed it should have been from my hand calculation. I solved for the length based on the given maximum deflection and the diameter I chose.

<p>(Simulated Deflection) <strong>&delta;</strong><sub>S</sub> = 0.0004974 in</p>
<p>(Deflection from Calculations) <strong>&delta;</strong><sub>M</sub> = 0.009 in</p>

<div align="center">
<strong>&delta;</strong><sub>M</sub> &minus; <strong>&delta;</strong><sub>S</sub> =
</div>

<div align="center">
0.009 in &minus; 0.0004974 in =
</div>

<div align="center">
<table style="border: 4px solid black;" cellpadding="10"><tr><td><strong>0.0085026 in</strong></td></tr></table>
</div>

A possible reason for a difference in the calculations is that the maximum deflection of 0.009 inches rounded up to 0.01 inches in the global variables table of SolidWorks. Another reason may be that the elasticity in the global variables section was exactly 10 × 10⁶ psi while the elasticity of 6061-T6 (SS) aluminum was 7604 psi higher than that.    

