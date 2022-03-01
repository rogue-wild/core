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
> - The most common error detection code used is the `parity bit`. A parity bit is an extra bit included with a binary message to make the total number of 1's either odd or even. A message of three bits and two possible parity bits is shown in Table. The P(odd) bit is chosen in such a way as to make the sum of 1's (in all four bits) odd. The P(even) bit is chosen to make the sum of all 1's even. In either case, the sum is taken over the message and the P bit. In any particular application, one or the other type of parity will be adopted. The even-parity scheme has the disadvantage of having a bit combination of all O's, while in the odd parity there is always one bit (of the four bits that constitute the message and P) that is 1. Note that the P(odd) is the complement of the P(even). 
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
>The organization of the computer is defined by its internal registers, the timing and control structure, and the set of instructions`(sequence of microoperations it performs on data stored in it's registers)` that it uses. 

>A computer instruction is a binary code that specifies a sequence of microoperations for the computer. Instruction codes together with data are stored in memory. The computer reads each instruction from memory and places it in a control register. The control then interprets the binary code of the instruction and proceeds to execute it by issuing a sequence of microoperations. Every computer has its own unique instruction set. The ability to store and execute instructions, the stored program concept, is the most important 
property of a general-purpose computer. 

An **instruction code** is a group of bits that instruct the computer to perform a specific operation. It is usually divided into parts, each having its own particular interpretation. The most basic part of an instruction code is its operation part. 

The **operation code** of an instruction is a group of bits that define such operations as add, subtract, multiply, shift, and complement. The number of bits required for the operation code of an instruction depends on the total number of operations available in the computer. The operation code must consist of at least n bits for a given 2^n (or less) distinct operations.

**Stored Program Organization**
>The simplest way to organize a computer is to have one processor register and an instruction code format with two parts. The first part specifies the operation to be performed and the second specifies an address. The memory address tells the control where to find an operand in memory. This operand is read from memory and used as the data to be operated on together with the data stored in the processor register.

>Instructions are stored in one section of memory and data in another. For a memory unit with 4096 words we need 12 bits to specify an address since 2^12 = 4096. If we store each instruction code in one 16-bit memory word, we have available four bits for the operation code (abbreviated opcode) to specify one out of 16 possible operations, and 12 bits to specify the address of an operand. The control reads a 16-bit instruction from the program portion of memory. It uses the 12-bit address part of the instruction to read a 16-bit operand from the data portion of memory. It then executes the operation specified by the operation code.

**Accumulator**
>Computers that have a single-processor register usually assign to it the name accumulator and label it AC. The operation is performed with the memory operand and the content of AC. If an operation in an instruction code does not need an operand from memory, the rest of the bits in the instruction can be used for other purposes. For example, operations such as clear AC, complement AC, and increment AC operate on data stored in the AC register. They do not need an operand from memory. For these types of operations, the second part of the instruction code (bits 0 through 11) is not needed for specifying a memory address and can be used to specify other operations for the computer. 

**Indirect Address**
>It is sometimes convenient to use the address bits of an instruction code not as an address but as the actual operand. When the second part of an instruction code specifies an operand, the instruction is said to have an immediate operand. When the second part specifies the address of an operand, the instruction is said to have a _direct address_. This is in contrast to a third possibility called _indirect address_, where the bits in the second part of the instruction designate an address of a memory word in which the address of the operand is found. One bit of the instruction code can be used to distinguish between a direct and an indirect address.

>The indirect address instruction needs two references to memory to fetch an operand. The first reference is needed to read the address of the operand; the second is for the operand itself. We define the _effective address_ to be the address of the operand in a computation-type instruction or the target address in a branch-type instruction.

**Computer Registers**
>Computer instructions are normally stored in consecutive memory locations and are executed sequentially one at a time. The control reads an instruction from a specific address in memory and executes it. It then continues by reading the next instruction in sequence and executes it, and so on. This type of instruction sequencing needs a counter to calculate the address of the next instruction after execution of the current instruction is completed. It is also necessary to provide a register in the control unit for storing the instruction code after it is read from memory. The computer needs processor registers for manipulating data and a register for holding a memory address.

**Timing and Control**
>The timing for all registers in the basic computer is controlled by a master clock generator. The clock pulses are applied to all flip-flops and registers in the system, including the flip-flops and registers in the control unit. The clock pulses do not change the state of a register unless the register is enabled by a control signal. The control signals are generated in the control unit and provide control inputs for the multiplexers in the common bus, control inputs in processor registers, and microoperations for the accumulator. There are two major types of control organization: hardwired control and microprogrammed control. In the hardwired organization, the control logic is 
implemented with gates, flip-flops, decoders, and other digital circuits. It has the advantage that it can be optimized to produce a fast mode of operation. In the microprogrammed organization, the control information is stored in a control memory. The control memory is programmed to initiate the required sequence of microoperations. A hardwired control, as the name implies, requires changes in the wiring among the various components if the design has to be modified or changed. In the microprogrammed control, any required changes or modifications can be done by updating the microprogram in control memory.

**Instruction Cycle**
>A program residing in the memory unit of the computer consists of a sequence of instructions. The program is executed in the computer by going through a cycle for each instruction. Each instruction cycle in turn is subdivided into a sequence of subcycles or phases. In the basic computer each instruction cycle consists of the following phases: 
>1. Fetch an instruction from memory. 
>2. Decode the instruction. 
>3. Read the effective address from memory if the instruction has an indirect address. 
>4. Execute the instruction. 
>Upon the completion of step 4, the control goes back to step 1 to fetch, decode, and execute the next instruction. This process continues indefinitely unless a HALT instruction is encountered.

**Fetch and Decode**
>Initially, the program counter PC is loaded with the address of the first instruction in the program. The sequence counter SC is cleared to 0, providing a decoded timing signal T0. After each clock pulse, SC is incremented by one, so that the timing signals go through a sequence T0, T1, T2, and so on. The rnicrooperations for the fetch and decode phases can be specified by the following register transfer statements. 

**Memory-Reference Instructions**
>In order to specify the rnicrooperations needed for the execution of each 
instruction, it is necessary that the function that they are intended to perform 
be defined precisely. 


**Input-Output Instructions**
>Input and output instructions are needed for transferring information to and from AC register, for checking the flag bits, and for controlling the interrupt facility.

**Program Interrupt**
>The process of communication just described is referred to as programmed control transfer. The computer keeps checking the flag bit, and when it finds it set, it initiates an information transfer. The difference of information flow rate between the computer and that of the input-output device makes this type of transfer inefficient. To see why thisis inefficient, consider a computer that can go through an instruction cycle in lμs. Assume that the input-output device can transfer information at a maximum rate of 10 characters per second. This is equivalent to one character every 100,000μs. Two instructions are executed when the computer checks the flag bit and decides not to transfer the information. This means that at the maximum rate, the computer will check the flag 50,000 times between each transfer. The computer is wasting time while checking the flag instead of doing some other useful processing task. An alternative to the programmed controlled procedure is to let the external device inform the computer when it is ready for the transfer. In the meantime the computer can be busy with other tasks. This type of transfer uses the interrupt facility. While the computer is running a program, it does not check the flags. However, when a flag is set, the computer is momentarily interrupted from proceeding with the current program and is informed of the fact that a flag has been set. The computer deviates momentarily from what it is doing to take care of the input or output transfer. It then returns to the current program to continue what it was doing before the interrupt. The interrupt enable flip-flop lEN can be set and cleared with two instructions. When lEN is cleared to 0 (with the !OF instruction), the flags cannot interrupt the computer. When lEN is set to 1 (with the ION instruction), the computer can be interrupted. These two instructions provide the programmer with the capability of making a decision as to whether or not to use the interrupt facility.

**Interrupt cycle**
>The interrupt cycle is a hardware implementation of a branch and save return address operation. The return address available in PC is stored in a specific location where it can be found later when the program returns to the instruction at which it was interrupted. This location may be a processor register, a memory stack, or a specific memory location. Here we choose the memory location at address 0 as the place for storing the return address. Control then inserts address 1 into PC and clears lEN and R so that no more interruptions can occur until the interrupt request from the flag has been serviced. 

#

## Assembler
>An assembler is a program that accepts a symbolic language program and produces its binary machine language equivalent. The input symbolic program is called the source program and the resulting binary program is called the object program. The assembler is a program that operates on character strings and produces an equivalent binary interpretation.

**Subroutines**
>Frequently, the same piece of code must be written over again in many different parts of a program. Instead of repeating the code every time it is needed, there is an obvious advantage if the common instructions are written only once. A set of common instructions that can be used in a program many times is called a subroutine. Each time that a subroutine is used in the main part of the program, a branch is executed to the beginning of the subroutine. After the subroutine has been executed, a branch is made back to the main program. A subroutine consists of a self-contained sequence of instructions that carries out a given task. A branch can be made to the subroutine from any part of the main program. This poses the problem of how the subroutine knows which location to return to, since many different locations in the main program may make branches to the same subroutine. It is therefore necessary to store the return address somewhere in the computer for the subroutine to know where to return. Because branching to a subroutine and returning to the main program is such a common operation, all computers provide special instructions to facilitate subroutine entry and return. 

#

## Control Memory






























































































































































































































































































































