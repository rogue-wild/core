# **Basics of Computer System**
<hr>

## **Digital Computers**
>The word digital implies that the information in the computer is represented by variables that take a limited number of discrete values. In practice, digital computers work reliably if only two states are used, because of physical restrictions and human logic tends to be bianry(Yes or No, True or False).
>A binary digit is called a bit. 

## **Program**
>A sequence of instructions for the computer is called a Program.

<img src="https://user-images.githubusercontent.com/42809447/155906712-cc5d455c-61bb-40ac-b9fd-3a781bdad433.png" height="400">

`Block Diagram of a Digital Computer`

#

## **Computer Organization**
>It is concerned with the way the hardware components operate and the way they are connected together to form the computer system.

## **Computer Design**
>It is concerned with the hardware design of the computer.

## **Computer Architecture**
>It is concerned with the structure and behaviour of the computer as seen by the user. It includes the information, the instruction set, and techniques for adressing memory. The architectural design of a computer system is concerned with the specifications of various functional modules, such as processors and memmories, and structuring them together in a computer system.

>Two basic types architecture are : 
>1. von Neumann Architecutre: _Von Neumann Architecture is a digital computer architecture whose design is based on the concept of stored program computers where program data and instruction data are stored in the same memory. This principle holds that data, as well as the instructions used to manipulate that data, should be stored in the same memory area of the computer and instructions are carried out sequentially, one instruction at a time. This imposes a sort of "speed limit" on program execution, since only on instruction at a time can be handled by the computer's processor. It means that the CPU can be either reading an instruction or reading/writing data from/to the memory. Both cannot occur at the same time since the instructions and data use the same signal pathways and memory. Eg.: PC(Personal Computers)_

<img src="https://user-images.githubusercontent.com/42809447/155906259-862ea1ed-22fa-4d41-ac10-64eba579d878.png" height="500"> 


>2. Harvard Architecutre: _Harvard Architecture is the computer architecture that contains separate storage and separate buses (signal path) for instruction and data. It was basically developed to overcome the bottleneck of Von Neumann Architecture. The main advantage of having separate buses for instruction and data is that the CPU can access instructions and read/write data at the same time. Eg.: Microcontrollers & DSP(Digital Signal Processors)_

<img src="https://user-images.githubusercontent.com/42809447/155906271-55c3bfb2-1262-42b2-862b-da7020d48ac9.png" height="500">


#

**Logic Gates**
> - Binary information is represented in digital computers by physical quantities called signals. Electrical signals such as voltages exist throughout the computer in either one of two recognizable states. The two states represent a binary variable that can be equal to 1 or 0.
> - Binary logic deals with binary variables and with operations that assume a logical meaning. It is used to describe, in algebraic or tabular form, the manipulation and processing of binary information. The manipulation of binary information is done by logic circuits called gates. Gates are blocks of hardware that produce signals of binary 1 or 0 when input logic requirements are satisfied. A variety of logic gates are commonly used in digital computer systems.

**Decoders**
>Discrete quantities of information are represented in digital computers with binary codes. A binary code of n bits is capable of representing up to 2^n distinct elements of the coded information. A decoder is a combinational circuit that converts binary information from the n coded inputs to a maximum of 2^n unique outputs. If the n-bit coded information has unused bit combinations, the decoder may have less than 2^n outputs. The decoders presented in this section are called n-to-m-line decoders, where < or equal to 2^n. Their purpose is to generate the 2^n (or fewer) binary combinations of the n input variables. A decoder has n inputs and m outputs and is also referred to as an n x m decoder.

**Encoders** 
>An encoder is a digital circuit that performs the inverse operation of a decoder. An encoder has 2^n (or less) input lines and n output lines. The output lines generate the binary code corresponding to the input value.

**Multiplexers**
>A multiplexer is a combinational circuit that receives binary information from one of 2^n input data lines and directs it to a single output line. The selection of a particular input data line for the output is determined by a set of selection inputs. A 2^n-to-1 multiplexer has 2^n input data lines and n input selection lines whose bit combinations determine which input data are selected for the output. 

#

## **Registers**
> - A register is a group of flip-flops with each flip-flop capable of storing one bit of information. An n-bit register has a group of n flip-flops and is capable of storing any binary information of n bits. In addition to the flip-flops, a register may have combinational gates that perform certain data-processing tasks. In its broadest definition, a register consists of a group of flip-flops and gates that effect their transition. The flip-flops hold the binary information and the gates control when and how new information is transferred into the register.

> - **Shift register**: A register capable of shifting its binary information in one or both directions is called a shift register. The logical configuration of a shift register consists of a chain of flip-flops in cascade, with the output of one flip-flop connected to the input of the next flip-flop. All flip-flops receive common clock pulses that initiate the shift from one stage to the next.
> - **Binary Counters**: A register that goes through a predetermined sequence of states upon the application of input pulses is called a counter. The input pulses may be clock pulses or may originate from an external source. They may occur at uniform intervals of time or at random. Counters are found in almost all equipment containing digital logic. They are used for counting the number of occurrences of an event and are useful for generating timing signals to control the sequence of operations in digital computers.


## **Memory Unit**
> - A memory unit is a collection of storage cells together with associated circuits needed to transfer information in and out of storage. The memory stores binary information in groups of bits called words. A word in memory is an entity of bits that move in and out of storage as a unit. A memory word is a group of l's and O's and may represent a number, an instruction code, one or more alphanumeric characters, or any other binary-coded information. 
>A group of eight bits is called a byte.

> - _`The internal structure of a memory unit is specified by the number of words it contains and the number of bits in each word. Special input lines called address lines select one particular word. Each word in memory is assigned an identification number, called an address, starting from 0 and continuing with 1, 2, 3, up to 2^k - 1 where k is the number of address lines. The selection of a specific word inside the memory is done by applying the k-bit binary address to the address lines. A decoder inside the memory accepts this address and opens the paths needed to select the bits of the specified word`_

> Two major types of memories are used in computer systems: random access memory (RAM) and read-only memory (ROM). 

**Random Access Memory (RAM):** *In random-access memory (RAM) the memory cells can be accessed for information transfer from any desired random location. That is, the process of locating a word in memory is the same and requires an equal amount of time no matter where the cells are located physically in memory: thus the name "random access."It is used to store the programs and data being used by the CPU in real-time. The data on the random access memory can be read, written, and erased any number of times. RAM is a hardware element where the data being currently used is stored. It is a volatile memory. Types of RAM:*
- Static RAM, or (SRAM) which stores a bit of data using the state of a six transistor memory cell.
- Dynamic RAM, or (DRAM) which stores a bit data using a pair of transistor and capacitor which constitute a DRAM memory cell.

>Communication between a memory and its environment is achieved through data input and output lines, address selection lines, and control lines that specify the direction of transfer.The n data input lines provide the information to be stored in memory, and the n data output lines supply the information coming out of memory. The k address lines provide a binary number of k bits that specify a particular word chosen among the 2' available inside the memory. The two control inputs specify the direction of transfer desired.The two operations that a random-access memory can perform are the write and read operations. The write signal specifies a transfer-in operation and the read signal specifies a transfer-out operation. On accepting one of these control signals, the internal circuits inside the memory provide the desired function. The steps that must be taken for the purpose of transferring a new word to be stored into memory are as follows: 

>![image](https://user-images.githubusercontent.com/42809447/155907828-c8ba47ba-b125-4a8b-8249-e7e5af1bc9b4.png)

>1. Apply the binary address of the desired word into the address lines.
>2. Apply the data bits that must be stored in memory into the data input 
lines. 
>3. Activate the write input. 
>The memory unit will then take the bits presently available in the input data lines and store them in the word specified by the address lines. The steps that must be taken for the purpose of transferring a stored word out of memory are as follows: 
>1. Apply the binary address of the desired word into the address lines. 
>2. Activate the read input. 
>The memory unit will then take the bits from the word that has been selected by the address and apply them into the output data lines. The content of the selected word does not change after reading. 

**Read Only Memory (ROM):** *is a type of memory where the data has been prerecorded. Data stored in ROM is retained even after the computer is turned off ie, non-volatile. Types of ROM:*

- Programmable ROM, where the data is written after the memory chip has been created. It is non-volatile.
- Erasable Programmable ROM, where the data on this non-volatile memory chip can be erased by exposing it to high-intensity UV light.
- Electrically Erasable Programmable ROM, where the data on this non-volatile memory chip can be electrically erased using field electron emission.
- Mask ROM, in which the data is written during the manufacturing of the memory chip.

>A read-only memory (ROM) is a memory unit that performs the read operation only; it does not have a write capability. This implies that the binary information stored in a ROM is made permanent during the hardware production of the unit and cannot be altered by writing different words into it. Whereas a RAM is a general-purpose device whose contents can be altered during the computational process, a ROM is restricted to reading words that are permanently stored within the unit. The binary information to be stored, specified by the designer, is then embedded in the unit to form the reqttired interconnection pattern. ROMs come with special internal electronic fuses that can be "programmed" for a specific configuration. Once the pattern is established, it stays within the unit even when power is turned off and on again. 

>![image](https://user-images.githubusercontent.com/42809447/155907853-84c297c4-c703-46cb-ab3c-d8e262a32915.png)

>An m x n ROM is an array of binary cells organized into m words of n bits each. A ROM has k address input llnes to select one of 2^k = m words of memory, and n output lines, one for each bit of the word. An integrated circuit ROM may also have one or more enable inputs for expanding a number of packages into a ROM with larger capacity.
>The ROM does not need a read-control llne since at any given time, the output lines automatically provide the n bits of the word selected by the address value. Because the outputs are a function of only the present inputs (the address lines), a ROM is classified as a combinational circuit. In fact, a ROM is constructed internally with decoders and a set of OR gates. There is no need for providing storage capabilities as in a RAM, since the values of the bits in the ROM are permanently fixed. 
>ROMs find a wide range of applications in the design of digital systems. Basically, a ROM generates an input-output relation specified by a truth table. As such, it can implement any combinational circuit with k inputs and n outputs. When employed in a computer system as a memory unit, the ROM is used for storing fixed programs that are not to be altered and for tables of constants that are not subject to change. ROM is also employed in the design of control units for digital computers. As such, they are used to store coded information that represents the sequence of internal control variables needed for enabling the various operations in the computer. A control unit that utilizes a ROM to store binary control information is called a microprogrammed control unit. 

#
**Error Detection Codes**
>Binary information transmitted through some form of communication medium is subject to external noise that could change bits from 1 to 0, and vice versa. An error detection code is a binary code that detects digital errors during transmission. The detected errors cannot be corrected but their presence is indicated. The usual procedure is to observe the frequency of errors. If errors occur infrequently at random, the particular erroneous information is transmitted again. If the error occurs too often, the system is checked for malfunction. 
> - The most common error detection code used is the `parity bit`. A parity bit is an extra bit included with a binary message to make the total number of 1's either odd or even. A message of three bits and two possible parity bits is shown in Table 3-7. The P(odd) bit is chosen in such a way as to make the sum of 1's (in all four bits) odd. The P(even) bit is chosen to make the sum of all 1's even. In either case, the sum is taken over the message and the P bit. In any particular application, one or the other type of parity will be adopted. The even-parity scheme has the disadvantage of having a bit combination of all O's, while in the odd parity there is always one bit (of the four bits that constitute the message and P) that is 1. Note that the P(odd) is the complement of the P(even). 
>
| Message *xyz* | P(odd)  | P(even)|
| :---          |:----:   |   ---: |
| 000           | 1       | 0      |
| 001           | 0       | 1      |
| 010           | 0       | 1      |
| 011           | 1       | 0      |
| 100           | 0       | 1      |
| 101           | 1       | 0      |
| 110           | 1       | 0      |
| 111           | 0       | 1      |


> - During transfer of information from one location to another, the parity bit is handled as follows. At the sending end, the message (in this case three bits) is applied to a `parity generator`, where the required parity bit is generated. 

> - The message, including the parity bit, is transmitted to its destination. At the receiving end, all the incoming bits (in this case, four) are applied to a `parity checker` that checks the proper parity adopted (odd or even). An error is detected if the checked parity does not conform to the adopted parity. The parity method detects the presence of one, three, or any odd number of errors. An even number of errors is not detected. 

**Register Transfer Language**
>In computer science, register transfer language is a type of object code a kind of intermediate representation that is very close to assembly language, such as that which is used in a compiler. It is used to describe data flow at the register-transfer level of an architecture.

**Register Transfer**
> Computer registers are designated by capital letters (sometimes followed by numerals) to denote the function of the register. For example, the register that holds an address for the memory unit is usually called a memory address register and is designated by the name MAR. Other designations for registers are PC (for program counter), IR (for instruction register, and R 1 (for processor register). The individual flip-flops in an n-bit register are numbered in sequence from 0 through n - 1, starting from 0 in the rightmost position and increasing the numbers toward the left. The most common way to represent a register is by a rectangular box with the name of the register inside. The statement 
> `R2 <-- R1` 
>denotes a transfer of the content of register R1 into register R2. It designates a replacement of the content of R2 by the content of Rl. By definition, the content of the source register R1 does not change after the transfer. 

**Bus and Memory Transfers**
>A typical digital computer has many registers, and paths must be provided to transfer information from one register to another. The number of wires will be excessive if separate lines are used between each register and all other registers in the system. A more efficient scheme for transferring information between registers in a multiple register configuration is a common bus system. A bus structure consists of a set of common lines, one for each bit of a register, through which binary information is transferred one at a time. Control signals determine which register is selected by the bus during each particular register transfer. 

#

## **Instruction Codes**

