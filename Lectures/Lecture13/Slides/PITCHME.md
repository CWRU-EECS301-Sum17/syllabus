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

* All FPGA signals require timing constraints
* Timing constraints set the allowed propagation time between registers
* Insuring register setup and hold times prevent metastability
* Constraints are used when mapping RTL logic onto the FPGA fabric

---

### Quartus Timing Constraints

* Quartus constraint files have an **.sdc** extension
* Every lab project has had a constraints file included
* TimeQuest Timing Analyzer provides timing reports
* Refer to this [User Guide](http://www.alterawiki.com/uploads/3/3f/TimeQuest_User_Guide.pdf) for detailed information about setting constraints in Quartus

---

### Clock Constraints

* Clock Constraints must be provided
* All registered signals reference a Clock
* Quartus can derive signal constraints automatically from the Clock constraint

---?image=https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture13/Slides/images/Clock_Constraint_Example.png&size=auto 90%

---

#### Quartus Constraints GUI

* Graphical interface to create constraints

![Create Clock GUI](https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture13/Slides/images/Timing_Create_Clock.png)

---

#### Input/Output Signal Constraints

---

### Other Constraints

* Multi-cycle
* False Paths
* Clock Relationships
* 

---

# Questions


