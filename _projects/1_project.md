---
layout: page
title: Mechanical and Thermal Stress Analysis of Different Types of Memory Chips
description: with background image
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
---

From the beginning of the era of technology, residual stress and high compressive stress formation in the chip during fabrication has remain a great problem. In this analysis, the compressive stress formation during different stages of fabrication and the final residual stress has been calculated using finite element method. Then a comparative analysis has been made between them. Among the two memory chips, less stress is formed in DRAM compared to NAND memory chip. In the later part, thermal stress analysis of the DRAM and NAND memory chip is done. It has shown that the stress in DRAM changes more linearly than NAND due to the effect of high residual stress in NAND.



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
<h3 class="mb-2">Step 1: VLSI Modeling</h3>

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
