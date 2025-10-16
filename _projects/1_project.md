---
layout: page
title: project 1
description: with background image
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
---

From the beginning of the era of technology, residual stress and high compressive stress formation in the chip during fabrication has remain a great problem. In this analysis, the compressive stress formation during different stages of fabrication and the final residual stress has been calculated using finite element method. Then a comparative analysis has been made between them. Among the two memory chips, less stress is formed in DRAM compared to NAND memory chip. In the later part, thermal stress analysis of the DRAM and NAND memory chip is done. It has shown that the stress in DRAM changes more linearly than NAND due to the effect of high residual stress in NAND.



The fabrication process for NAND, DRAM and VNAND are different and each process is subjected to different thermal loading conditions. This loading condition gives rise to stress which can remain present even after the fabrication is done. 


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/thesis_temp_vnand.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Temperature variation with different fabrication steps in VNAND fabrication
</div>

You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

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
        A tunnel oxide layer and a first polysilicon layer for floating gate, a buffer oxide and a nitride layer are subsequently deposited on a Silicon substrate at 700 and 720 C respectively. Portioned of the nitride layer, first polysilicon layer, tunnel oxide and silicon substrate are selectively etched at room temperature and trenches are formed on the silicon substrate.  An insulating oxide layer is formed in the trenches. Then the buffer oxide and a portion of insulating layer is striped. After that a second polysilicon layer is deposited at 700C. Then the top potion of the second polysilicon is etched and a dielectric layer is formed on it. Then finally the conduction metal is deposited at 350C.
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/thesis_processflow_NAND.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Process Flow Diagram of NAND memory cell.
</div>

This variation of fabrication steps and temperatures give rises to stress inside the chip which can cause both mechanical and electrical failure. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:



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
