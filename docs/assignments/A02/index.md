# A2 – Truss Stress Analysis

## Objective

My objective is to design and 3D model a truss system out of A36 steel that can support the load within the provided scenario.

<div style="text-align: center;">
  <img src="ProvideScenerio.jpg" alt="Clap Photo 2">
</div>

<div style="text-align: center;">
  <p style="font-weight: bold; margin: 8px 0;"><b>Y<sub>s</sub> = 250 MPa</b></p>
  <p style="font-weight: bold; margin: 8px 0;"><b>P = 20 kN</b></p>
  <p style="font-weight: bold; margin: 8px 0;"><b>a = 0.3 m</b></p>
  <p style="font-weight: bold; margin: 8px 0;"><b>b = 0.3 m</b></p>
</div>

## Design Process

The two things I immediately thought of when I was deciding how to design my truss system was stability and triangulation. I know that triangles are one of the strongest planar structures and I know the formula that for how many joints should be in a truss for it to be statically determinate. Utilizing this formula, I concluded that I should 5 members in my system.

<div style="text-align: center;">
  <p style="font-weight: bold; margin: 8px 0;">2⋅(# of joints) = 3 + (# of members)</p>
  <p style="font-weight: normal; margin: 20px 0;">-2(4) = 3 + x</p>
  <p style="display: inline-block; border: 1px solid #000; padding: 4px 12px; margin: 8px 0; font-weight: normal;">x = 5</p>
</div>

<div style="text-align: center;">
  <img src="Truss1.jpg" alt="Clap Photo 2">
</div>

## External Forces

<div style="text-align: left;">

  <p><b>ΣF<sub>y</sub></b> = 0 = A<sub>y</sub> + B<sub>y</sub> − P + P</p>
  <p style="text-align: center; font-weight: bold; display: block;">
    <span style="display: inline-block; border: 1px solid #000; padding: 4px 12px;">A<sub>y</sub> = −B<sub>y</sub></span>
  </p>

  <p><b>ΣF<sub>x</sub></b> = 0 = A<sub>x</sub></p>
  <p style="text-align: center; font-weight: bold; display: block;">
    <span style="display: inline-block; border: 1px solid #000; padding: 4px 12px;">A<sub>x</sub> = 0</span>
  </p>

  <p><b>ΣM<sub>A</sub></b> = 0 = +P(a) − P(2a) + B<sub>y</sub>(3a)</p>
  <p>B<sub>y</sub>(3a) = P(a − 2a)</p>
  <p>B<sub>y</sub>(3a) = P(−a)</p>
  <p style="text-align: center; font-weight: bold; display: block;">
    <span style="display: inline-block; border: 1px solid #000; padding: 4px 12px;">B<sub>y</sub> = −P(1/3)</span>
  </p>

</div>

## Decide
_Which geometry did you select, and why? This is your first open design choice in the course — defend it._

## Communicate

