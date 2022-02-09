# Parallel-In-Serial-Out-Shift-Register
* Design and implementation of Synchronous Parallel In Serial Out Shift Register which is used to convert parallel data to serial data . Shift register also acts as a temporary storage device. it can be used to multiplex different data lines into a single line which makes it easy to transmit over a single line.

# Table of Contents

1.[ Introduction](#Introduction)

2.[ INSTALLATION OF TOOLS](#INSTALLATION-OF-TOOLS)

3.[ Circuit Design and Details](#Circuit-Design-and-Details)

3.[ Circuit Operation](#Circuit-Operation)
   
4.[ Simulation Waveforms](#Simulation-Waveforms)

5.[ Conclution](#Conclution)

6.[ References](#References)

7.[ Acknowledgement](#Acknowledgement)

8.[ Author](#Author)

## Introduction




## INSTALLATION OF TOOLS
***
#### esim:
esim is an open-source EDA tool used for circuit design and simulation. Using esim we can draw circuit using Kicad, generate netlist and simulate using Ngspice.

For more information: <https://esim.fossee.in/home>

#### Ngspice:

ngspice is the open-source spice simulator for electric and electronic circuits. We can design circuits using JFET, MOSFET and passive elements like resistors, capacitors, etc.

For more information: <http://ngspice.sourceforge.net>

#### Sky130nm PDK:

The SkyWater Open Source PDK is a collaboration between Google and SkyWater Technology Foundry to provide a fully open source Process Design Kit and related resources, which can be used to create manufacturable designs at SkyWater’s facility. 

For more information: <https://www.layouteditor.org/schematiceditor/libraries/skywater>

The Download links for above software are:

#### esim: <https://esim.fossee.in/downloads>

#### Ngspice: <https://sourceforge.net/projects/ngspice/files/>

#### Sky130 pdk: <https://static.fossee.in/esim/installation-files/sky130_fd_pr.zip>


## Circuit Design and Details

#### Schematic Diagram of FISO shift Register
![piso ](https://user-images.githubusercontent.com/67550103/153134866-392da811-84db-4f1e-bfc4-81c0c2d480c5.png)
#### Schematic Diagram of inverter
![inv](https://user-images.githubusercontent.com/67550103/153133705-80cf44ff-848a-448d-a6dd-ca42cf84bcb5.png)
#### Schematic Diagram of And logic gate
![and](https://user-images.githubusercontent.com/67550103/153133702-f8241e53-e737-49c9-9d69-c00158a35d89.png)
#### Schematic Diagram of Or logic gate
![or](https://user-images.githubusercontent.com/67550103/153133709-16dda94c-29d3-4dd9-9e94-46fa1d69bc1a.png)
#### Schematic Diagram of D-flip flop
![dff](https://user-images.githubusercontent.com/67550103/153133700-6bb16db5-29b5-47ee-a7a3-9c079d2e0c97.png)


## Circuit Operation


## Simulation Waveforms


## Conclution



![waveform ](https://user-images.githubusercontent.com/67550103/153132397-1410e090-d453-492f-9405-de9a24f5f52b.jpg)



## References

* Namrata Joshi. "Design and Analysis of High Performance PISO & PIPO Shift Registers." IOSR Journal of Electronics and Communication Engineering (IOSR-JECE) 14.2 (2019)
*  Shift Registers in Digital Logic https://www.geeksforgeeks.org/shift-registers-in-digitallogic/
* Parallel-in Serial-out Shift Register (PISO) https://instrumentationtools.com/topic/parallel-in-serialout-shift-register-piso/
## Acknowledgement

Kunal Ghosh,Co-founder of VLSI System Design Corporation Pvt. Ltd.

## Author

Chinmaya Nilakantha Naik , Final Year B.E, ECE, Mangalore Institute of technology and Engineering

Email: chinmayanaik920@gmail.com
