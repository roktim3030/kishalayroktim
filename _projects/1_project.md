---
layout: page
title: Mechanical and Thermal Stress Analysis of Different Types of Memory Chips
description: with background image
img: assets/img/12.jpg
importance: 1
category: work
related_publications: false
---

<h2 class="mt-4 mb-3">Abstract</h2>
From the beginning of the era of technology, residual stress and high compressive stress formation in the chip during fabrication has remain a great problem. In this analysis, the compressive stress formation during different stages of fabrication and the final residual stress has been calculated using finite element method. Then a comparative analysis has been made between them. Among the two memory chips, less stress is formed in DRAM compared to NAND memory chip. In the later part, thermal stress analysis of the DRAM and NAND memory chip is done. It has shown that the stress in DRAM changes more linearly than NAND due to the effect of high residual stress in NAND.


<h2 class="mt-4 mb-3">Introduction</h2>

The fabrication process for NAND, DRAM and VNAND are different and each process is subjected to different thermal loading conditions. This loading condition gives rise to stress which can remain present even after the fabrication is done.



<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        A tunnel oxide layer and a first polysilicon layer for floating gate, a buffer oxide and a nitride layer are subsequently deposited on a Silicon substrate at 700 and 720 C respectively. Portioned of the nitride layer, first polysilicon layer, tunnel oxide and silicon substrate are selectively etched at room temperature and trenches are formed on the silicon substrate.  An insulating oxide layer is formed in the trenches. Then the buffer oxide and a portion of insulating layer is striped. After that a second polysilicon layer is deposited at 700C. Then the top potion of the second polysilicon is etched and a dielectric layer is formed on it. Then finally the conduction metal is deposited at 350C.
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/thesis_processflow_NAND.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Process Flow Diagram of NAND memory cell.
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        The simulation of VNAND chip is done for validation of the workflow. We can get the value of Final Residual stress in the Polysilicon and Tungsten layer. Then we follow the process flow given in the Figure 3-2 and calculate the final residual stress in the VNAND chip. From the figure, we can see how the temperature varies with different fabrication steps. Maximum temperature during deposition occurs during the deposition of nitride at 800°. At the end of the fabrication steps, when the temperature returns to room temperature the final residual is found. 
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/thesis_processflow_VNAND.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Process Flow Diagram of NAND memory cell.
</div>

This variation of fabrication steps and temperatures give rises to stress inside the chip which can cause both mechanical and electrical failure. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/thesis_temp_vnand.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Temperature variation with different fabrication steps in VNAND fabrication
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/thesis_temp_DRAM.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/thesis_temp_nand.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/thesis_temp_vnand.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Temperature variation with different fabrication steps in a. DRAM fabrication b. NAND fabrication c. VNAND fabrication
</div>

<h2 class="mt-4 mb-3">Methodology</h2>
The methodology of this thesis is mainly divided into two parts, The electrical part and the finite element stress analysis. For the electrical part of this research, an electronic design software named Microwind is used and then for the mechanical analysis, the model is at first prepared using Solidworks and then the stress analysis is done using Finite element analysis by Ansys.

<h3 class="mb-2">VLSI Solidworks Modeling</h3>
At first, the layouts of VNAND, DRAM, and conventional NAND memory chips are created and simulated using Microwind, electronic design automation tool. The schematic design is the first step in the process, where necessary components are placed to create the fundamental circuit. Subsequently, the layout design takes place, encompassing the definition of layers, arrangement of components, and routing of the metal wire following the design rules. By optimizing the design for better performance and manufacturability, the iterative refinement process makes sure that the memory chips satisfy all requirements. One DRAM cell and two NAND memory cells with 0.12μm and 0.06μm is prepared. Here the red line represents Polysilicon, Indigo represents Metal wire connection and Royal Blue represents Metal2 wire. Polysilicon is directly placed on the silicon substrate. Metal1 is connected to Silicon substrate using Contacts and the metal2 is connected to metal1 using metal VIA. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/thesis_DRAM_microwind.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/thesis_DRAM_solidworks.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Model Preparation of DRAM memory cell for simulation using a. microwind b. solidworks
</div>

<h3 class="mb-2">Finite Element Analysis</h3>

The finite element method (FEM) was employed to model the mechanical and thermal stress evolution within the multilayer structures of DRAM, NAND, and VNAND memory chips during fabrication. The analysis was performed using a 3D model to reduce computational cost while maintaining physical accuracy. Each material layer—such as silicon substrate, oxide, nitride, polysilicon, tungsten, and copper interconnect—was defined according to its respective thickness and material properties, as listed in Table 1.

The simulation used temperature-dependent boundary conditions to represent the sequential deposition and etching steps in the fabrication process. A thermal loading profile was applied to each layer according to the specific deposition temperature, followed by natural cooling to room temperature (25 °C). The residual stress generated from the difference in the coefficients of thermal expansion among materials was calculated during each step.

To ensure mesh convergence and accuracy, finer meshing was applied near material interfaces where steep stress gradients occur. The bottom of the silicon substrate was constrained in all directions to mimic the fixed boundary of the wafer, while the top surface was left free to deform. 

Post-processing included the evaluation of:
- Minimum principal stress and maximum shear stress distributions at different components,  
- Stress variation with temperature is analyzed, and  
- residual stress after the final cooldown step.  

The FEM results were then compared between DRAM, NAND, and VNAND structures to evaluate the effect of different fabrication temperatures and material combinations on final residual stress levels.

<h4 class="mt-4 mb-3">Material and Physical Parameters</h4>

<table class="table table-bordered table-striped text-center align-middle">
  <thead class="table-light">
    <tr>
      <th>Material</th>
      <th>Coefficient of Thermal Expansion (×10⁻⁶ /K)</th>
      <th>Young’s Modulus, E (GPa)</th>
      <th>Poisson’s Ratio (ν)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Silicon</td>
      <td>3.1</td>
      <td>162</td>
      <td>0.28</td>
    </tr>
    <tr>
      <td>Oxide</td>
      <td>1</td>
      <td>70</td>
      <td>0.24</td>
    </tr>
    <tr>
      <td>Nitride</td>
      <td>2.8</td>
      <td>260</td>
      <td>0.23</td>
    </tr>
    <tr>
      <td>Polysilicon</td>
      <td>3</td>
      <td>160</td>
      <td>0.22</td>
    </tr>
    <tr>
      <td>Tungsten</td>
      <td>4.1</td>
      <td>410</td>
      <td>0.28</td>
    </tr>
    <tr>
      <td>Copper</td>
      <td>17</td>
      <td>110</td>
      <td>0.34</td>
    </tr>
  </tbody>
</table>



{% raw %}
```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```
{% endraw %}
