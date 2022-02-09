# Parallel-In-Serial-Out-Shift-Register
* Design and implementation of Synchronous Parallel In Serial Out Shift Register which is used to convert parallel data to serial data . Shift register also acts as a temporary storage device. it can be used to multiplex different data lines into a single line which makes it easy to transmit over a single line.

# Table of Contents

1.[ Introduction](#Introduction)

2.[ InstallationOf Tool's ](#InstallationOf-Tool's )

3.[ Circuit Design](#Circuit-Design)

4.[ Circuit Operation](#Circuit-Operation)
   
5.[ Simulation Waveforms](#Simulation-Waveforms)

6.[ References](#References)

7.[ Acknowledgement](#Acknowledgement)

8.[ Author](#Author)

## Introduction
Parallel In Serial Out Shift Register which is used to convert parallel data to serial data. Shift Register is a group of flip flops that is used to store or move the multiple bits of data. In the Parallel In Serial Out (PISO) shift register the data is shifted Parallely ‘IN’ and serially ‘OUT’ of the register, one bit at a time in either a left or right direction under clock control.Simultaneously Data is loaded into the register. There is only one output to the PISO, In a serial pattern the data leaves the shift register one bit at a time. The circuit consists of four D flip-flops which are connected in a serial manner also or, and & not logic gates. Since the same clock signal is applied to each flip flop, All these flip-flops are synchronous with each other. This reference circuit will be simulated in eSim EDA tool and then will be implemented using SkyWater’s 130nm PDK.


***
## InstallationOf Tool's 

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

***
## Circuit Design

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


***
## Circuit Operation
Shift register is a group of flip flops arranged in a manner to shift the data stored in the FF to the next FF for every clock pulse.The data is loaded into the register in a parallel format which means all of the data bits enter their inputs simultaneously to the parallel input pins D0 to D3 of the register. To load the data into all registers only one clock pulse is enough but four clock pulses are required to shift and unload the data from the registers.The FISO circuit consists of four D flip-flops which are connected in serial fashion. The clock input is directly given to all the flip flops but the input data is connected individually to each flip flop through a MUX.The output of the previous flip flop and parallel data from the input are connected to the inputs of the MUX and t MUX output is connected to the next flip flop.Each flip flop has a respective input from D0 to D3. If the control signal Shift =0 then each flip flop is loaded with input. If the control signal Shift =1 then shifting has performed and output has taken from the last flip flop serially.When the Shift is logic high. The lower AND gates of the pairs feeding the OR gate are enabled that makes a connection of Q0 to D1 , Q1 to D2 , Q2 to D3 . Clock pulses will make data to shift right and finally out of D3 on successive pulses.
***
## Simulation Waveforms
![waveform ](https://user-images.githubusercontent.com/67550103/153132397-1410e090-d453-492f-9405-de9a24f5f52b.jpg)


***
## References

* Namrata Joshi. "Design and Analysis of High Performance PISO & PIPO Shift Registers." IOSR Journal of Electronics and Communication Engineering (IOSR-JECE) 14.2 (2019)
*  Shift Registers in Digital Logic https://www.geeksforgeeks.org/shift-registers-in-digitallogic/
* Parallel-in Serial-out Shift Register (PISO) https://instrumentationtools.com/topic/parallel-in-serialout-shift-register-piso/
***
## Acknowledgement

Kunal Ghosh,Co-founder of VLSI System Design Corporation Pvt. Ltd.
***
## Author

Chinmaya Nilakantha Naik , Final Year B.E, ECE, Mangalore Institute of technology and Engineering

Email: chinmayanaik920@gmail.com
