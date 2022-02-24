# 4-bit-Binary-to-Gray-converter
This repository presents the design of 4-bit BINARY TO GRAY CONVERTER implemented using Synopsis Custom Compiler on 28nm CMOS Technology.

# Table of contents:
 * [Introduction](#Introduction)
 * [Binary to Gray Conversion Steps](#Converting-from-binary-to-grayscale)
 * [Tools Used](#Tools-Used)
 * [Simulation in Synopsys](#Simulation-in-Synopsys)
 * [Netlist of the Circuit](#Netlist-of-the-Circuit)
 * [Author](#Author)
 * [Acknowledgements](#Acknowledgements)
 * [References](#References)




# Introduction
Converting binary code to grey code is known as binary to grey conversion. This may produce an error during the transition from one number to the next in the typical series of binary numbers generated by the device. Because only one bit changes its value during any transition between two values, the Gray code can readily solve this problem. The most common application of Grey Code is in embedded systems, notably in counting; but, as automation in everyday gadgets and technology increases, so will the use of grey code as a whole.


## Converting from binary to grayscale:


The Binary to Gray Code Converter is a logical circuit that converts binary code into its Gray code equivalent. The n-bit grey code can be obtained by placing the MSB of 1 below the axis and the MSB of 1 above the axis, then reflecting the (n-1) bit code about an axis after 2n-1 rows.

The following is the 4-bit binary to grey code conversion table:

Decimal Number	4-bit Binary Code	4-bit Gray Code:


| Decimal | Binary(B3 B2 B1 B0) | Gray(G3 G2 G1 G0)|
| ------ | ------ |  ------ |
| 0 | 0000 | 0000 |
| 1 | 0001 | 0001 |
| 2 | 0010 | 0011 |
| 3 | 0011 | 0010 |
| 5 | 0100 | 0110 |
| 5 | 0101 | 0111 |
| 6 | 0110 | 0101 |
| 7 | 0111 | 0100 |
| 8 | 1000 | 1100 |
| 9 | 1001 | 1101 |
| 10 | 1010 | 1111 |
| 11 | 1011 | 1110 |
| 12 | 1100 | 1010 |
| 13 | 1101 | 1011 |
| 14 | 1110 | 1001 |
| 15 | 1111 | 1000 |







![binary-to-gray-code-converter-ckt](https://user-images.githubusercontent.com/100235259/155311927-7f023274-42e0-43ac-98ad-895c4b28f373.png)


Fig(a) Binary to Gray code conversion


## How to Change a Binary Code into a Gray Code


1)The MSB of a Gray code number is always the same as the first bit of the binary number.


2)To perform the second bit of the grey code, we use the exclusive-or (XOR) of the binary number's first and second bits. If both bits are different, the outcome will be one; otherwise, the result will be 0.


3)To obtain the 3rd bit of the grey code, we must conduct an exclusive-or (XOR) operation on the binary number's 2nd and 3rd bits. For the 4th bit of the Gray code, the procedure is the same. To further comprehend these stages, consider the following scenario.

The output equtions are:-

```sh

G0=B0 xor B1

G1=B1 xor B2

G2=G2 xor G3

G3=B3.

```


## Tools Used:


- Synopsys Custom Compiler:
The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.
 

- Synopsys Primewave:
PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.
 


- Synopsys 28nm PDK:
 The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.
 

# Simulation in Synopsys:
## Schamatic
![inverter](https://user-images.githubusercontent.com/100235259/155359719-88a9835f-2695-4904-be8d-c63103737981.png)

 Fig(b):INVERTER
 ***
 

![s_inv](https://user-images.githubusercontent.com/100235259/155359742-5e0fdd5d-51d8-4798-a829-e4cf8998b02f.png)

 Fig(c):SYMBOL OF INVERTER
******



![xor_sch](https://user-images.githubusercontent.com/100235259/155359904-be94619d-0cbb-4ded-96ad-bb22e6ce7e4d.png)

Fig(d):XOR GATE

*********


![xor_sym](https://user-images.githubusercontent.com/100235259/155359912-0088ffbe-7cc1-4ac4-bdff-745983cd00c7.png)

Fig(e):SYMBOL OF XOR GATE
************

![B2GGG (1)](https://user-images.githubusercontent.com/100235259/155491290-c029a518-c767-4dc3-a7b0-320a13392660.png)



Fig(f):SCHAMATIC OF BINARY TO GRAY CONVERTE
***********
# Output Waveform
![SCH1234 (1)](https://user-images.githubusercontent.com/100235259/155491342-d5f87958-45a6-40c9-afc1-9192e914122e.png)


Fig(g): Output waveform of 4-bit binary to gray converter


# Netlist of the Circuit



## Author
• Mansi Shukla, M.Tech(Vlsi and Embedded Systems), IIIT–Naya Raipur, Atal Nagar – 493661

# Acknowledgements
• <a href='https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/'>Cloud Based Analog IC Design Hackathon</a></br>
• <a href='https://www.synopsys.com/'>Synopsys India</a></br>
• <a href='https://www.vlsisystemdesign.com/'>VLSI System Design (VSD) Corp. Pvt. Ltd India</a></br>

# References
[1]Babu, P. Ashok, et al. "Realization of 8 x 4 Barrel shifter with 4-bit binary to Gray converter using FinFET for Low Power Digital Applications." Journal of Physics: Conference series. Vol. 1714. No. 1. IOP Publishing, 2021.
