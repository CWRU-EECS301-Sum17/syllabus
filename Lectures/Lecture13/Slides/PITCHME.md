# EECS301

## Week 13

### 12/1/2017

---

## Lab 10 Demo

![Demo](https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture13/Slides/images/Lab10_Demo.png)

---

## Lab 10 Questions

Note:
Lab 10 Questions, Issues, Feedback?

---

### Computation Pipelines

* Computational pipelining utilizes parallelism to increase throughput
* FPGA logic is massively parallel
* CPUs, GPUs, and DSPs have highly optimized but fixed pipelines
* FPGA pipelines are customizable per application

Note:
The pipelines in CPUs, GPUs, and DSPs are designed for a specific task and may outperform an FPGA running the equivalent task by increasing the clock rates past an FPGAs clocking limit due to the chip hardware layout.
FPGAs offer complete flexibility in the pipeline logic and multiple pipeline instances can increase the total throughput.

---

### Pipeline Algorithms

* Math Operations (Square Root, Polynomials, etc)
* Data Stream Processing (Conversions, Filtering)
* Graphics Rendering
* Real-time Control

---

### Key Pipeline Features

* Maximum throughput when pipeline is full
* Each stage passes complete results to the next stage
* Pass-thru signal registers maintain pipeline ordering
* FPGA pipeline stages typically complete in single clock cycle but multi-cycle stages are possible
* Stage propagation delays determine max clock rate

---?image=https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture13/Slides/images/Pipeline_Example.png&size=auto 90%

---

## Pipelining Questions?

---

### FPGA Timing Constraints

* FPGA designs require signal timing constraints to set the propagation delay time limits between registers
* Register setup and hold times are validated against the timing constraints
* Over-constraining a design causes longer compile times 

---

### Quartus Timing Constraints

* Quartus maps logic elements into the FPGA fabric based on the timing constraint propagation times
* Quartus constraint files have an **.sdc** extension
* Every lab project has had a constraints file included
* Timing reports provided by TimeQuest Timing Analyzer
* Refer to this [User Guide](http://www.alterawiki.com/uploads/3/3f/TimeQuest_User_Guide.pdf) for detailed information about setting constraints in Quartus

---

### Clock Constraints

* In synchronous designs all signals reference a Clock signal
* Providing the clock constraint is critical
* The clock constraint covers most of the signals in the design
* The DE1-SoC board's main clock input is 50 MHz

```
create_clock -name {CLOCK_50} -period 20.000 [get_ports {CLOCK_50}]
```

Note:
The clock name does not have to be the same as the port name.
All signal names are case-sensitive

---

### Quartus Constraints GUI

* Graphical interface to set and review timing constraints

![Create Clock GUI](https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture13/Slides/images/Timing_Create_Clock.png)

---


---


---


---


---

# Questions


