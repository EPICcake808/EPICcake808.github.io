---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "Custom 32-Bit ISA CPU"
date: 2022
published: true
labels:
  - Computer Architecture
  - ARM Assembly
  - Verilog
summary: "My team designed and implented a 32-Bit Custom ISA CPU."
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

I worked with a team of students to design and implement, from scratch, a functioning 32-bit custom instruction set architecture (ISA) CPU for my computer architecture class at Santa Clara University. The design and architecture was based on a modified MIPS architecture with specifications provided by the instructor. We first designed the CPU pipeline on paper with considerations made for the specifications provided by the instructor. The instruction fetch, instruction decode, execute, and writeback stages were all designed by me and my team. In our team, I was the primary programmer, writing the majority of the Verilog. I was also responsible for debugging the Verilog code and ensuring that the output using test programs (written in ARM Assembly) matched what was expected.

You can learn more at https://github.com/EPICcake808/COEN-122-Final-Project
