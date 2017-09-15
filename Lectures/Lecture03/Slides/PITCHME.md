---

# Lab 2 Review

Note:
Lab 2 Questions, Issues, Feedback?


---?image=https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture03/Slides/BadSimulation.png&size=90% 90%

Note:
Red signals are uninitialized registers

---

#### Uninitialized Registers

```verilog
reg [31:0] count_reg;

initial
begin
	count_reg <= 32'h00000000;
end

always @(posedge CLK)
begin
	count_reg <= count_reg + 1'b1;
end
```

---

### Asynchronous Signals



---

## Metastability Demo

---?image=https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture03/Slides/MetastabilityDemoCircuit.png&size=90% 90%

---

### SN74S74 Datasheet Parameters

![74S74 Specs](https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture03/Slides/Specs_SN74S74.png)

---

### Cyclone FPGA LE Parameters

![Cyclone Specs](https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture03/Slides/Specs_Cyclone.png)

---

### Synchronizer Register Chain

![Sync Chain](https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture03/Slides/SyncChain.png)

Note:
Typical synchronizer chain length is 2 or 3 registers.
Faster clock rates need longer chains due to metastability bleed though which is shown in the Faster Clock slide.
overflow

---?image=https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture03/Slides/MsWf01.png&size=auto 90%

---?image=https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture03/Slides/MsWf02.png&size=auto 90%

---?image=https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture03/Slides/MsWf02.png&size=auto 90%

---

## MTBF

mean time between failures


---

# Lab 3 Overview

---

### Refactoring Code

