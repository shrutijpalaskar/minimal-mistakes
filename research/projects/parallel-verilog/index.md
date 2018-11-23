---
layout: page
title:
tags: [research, satwik, kottur, cmu, graduate, iitb]
modified: 2014-09-08T20:53:07.573882-04:00
comments: false
---

### Parallel Simulation of Verilog HDL designs

*Internship, IIT Bombay, Summer 2012*  
Guide: Prof. Sachin Patkar  

Digital designs, before synthesis, are simulated on a computer platform to test their efficiency. Maximizing the performance and minimizing the overheads is, therefore, a vital area of research. The main focus of this work is to parallelize the simulation of single clock structural/behavior hardware designs without any time or resource conflict. Thus, resulting in a multi-fold in reduction in execution time.

<figure class="half">
    <a href="/images/digital-code.jpg"><img src="/images/digital-code.jpg"></a>
    <a href="/images/digital-graph.jpg"><img src="/images/digital-graph.jpg"></a>
    <figcaption>Sample Verilog design (left), equivalent graph representation (right).</figcaption>
</figure><br/>

Due to advancements in the multi-core precessors, it is possible to simulate parallelizable designs faster. The flow of the work is briefly given below:
<ol class="proj-points">
<li>A given hardware design is converted into a standard XML structure. This allows the feasibility of using any description language (Verilog, in this case) for multi-platform compatibility.</li>
<li>This XML structure can be parsed in any high level language (Python) using standard libraries.</li>
<li>The design is systematically analyzed in the high level language to find functionally independent units.</li>
<li>These independent components are launched as seperate threads on a multi-core platform resulting in an overall reduction in time of simulation.</li>
</ol>

I have been awarded **Undergraduate Research Award** (URA 01) for contribution to research at IIT Bombay for this work.
Since this work has been done in close association with a graduate student, most of the implementation details can be found in his thesis report <a href="/reports/Digital-Reference.pdf">here</a>.  
[[TOP](/research/projects/parallel-verilog/)][[BACK](/research/#parallel-simulation-of-verilog-hdl-designs)]
