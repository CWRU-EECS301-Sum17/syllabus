---

# Lab 9 Questions

Note:
Lab 9 Questions, Issues, Feedback?

---

### Signal Digitizer

* Capture digital waveforms to memory buffer
* Common applications
	* Oscilloscope
	* Data Acquisition 
	* Audio Recording

---

### Digitized Waveform

* Fixed interval sampling

![Sampled Waveform](https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture12/Slides/images/Sampled_Waveform.png)

Note:
* Fixed sample rate doesn't require time samples
* Variable sample rate requires time stamps time domain correlation

---

### SCPI Trigger Model

* Basis for most Instrumentation Trigger Systems
* SCPI Trigger Model Layers
	* Idle
	* Initiate
	* Arm
	* Trigger
	* Device Action
* http://www.ivifoundation.org/docs/scpi-99.pdf

Note:
Standard Commands for Programmable Instruments (SCPI)
IVI Foundation Standard
SCPI Standard defines Trigger Model used by many instrumentation products.
http://www.ivifoundation.org/docs/scpi-99.pdf

---?image=https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture12/Slides/images/TriggerModel.png&size=auto 90%

---?image=https://raw.githubusercontent.com/CWRU-EECS301-Sum17/syllabus/master/Lectures/Lecture12/Slides/images/TriggerModelSamplingExample.png&size=90% auto


---

## Clock Domains

* Large designs may contain multiple clock sources
* Clock Domain contains all logic synchronized by the clock source
* Metastable events can occur when passing signals between domains
* Use proper synchronization structures when crossing domains

---

## Pipeline Calculations

---

## Square Root

---

# Lab 9 Questions


