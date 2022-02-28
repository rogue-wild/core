# **Basics of Computer System**
**Digital Computers**
>The word digital implies that the information in the computer is represented by variables that take a limited number of discrete values. In practice, digital computers work reliably if only two states are used, because of physical restrictions and human logic tends to be bianry(Yes or No, True or False).
>A binary digit is called a bit. 

**Program**
>A sequence of instructions for the computer is called a Program.

<img src="https://user-images.githubusercontent.com/42809447/155906712-cc5d455c-61bb-40ac-b9fd-3a781bdad433.png" height="500">

`Block Diagram of a Digital Computer`

#

**Computer Organization**
>It is concerned with the way the hardware components operate and the way they are connected together to form the computer system.

**Computer Design**
>It is concerned with the hardware design of the computer.

**Computer Architecture**
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

**Registers**
> - A register is a group of flip-flops with each flip-flop capable of storing one bit of information. An n-bit register has a group of n flip-flops and is capable of storing any binary information of n bits. In addition to the flip-flops, a register may have combinational gates that perform certain data-processing tasks. In its broadest definition, a register consists of a group of flip-flops and gates that effect their transition. The flip-flops hold the binary information and the gates control when and how new information is transferred into the register.

> - **Shift register**: A register capable of shifting its binary information in one or both directions is called a shift register. The logical configuration of a shift register consists of a chain of flip-flops in cascade, with the output of one flip-flop connected to the input of the next flip-flop. All flip-flops receive common clock pulses that initiate the shift from one stage to the next.
> - **Binary Counters**: A register that goes through a predetermined sequence of states upon the application of input pulses is called a counter. The input pulses may be clock pulses or may originate from an external source. They may occur at uniform intervals of time or at random. Counters are found in almost all equipment containing digital logic. They are used for counting the number of occurrences of an event and are useful for generating timing signals to control the sequence of operations in digital computers.


**Memory Unit**
> - A memory unit is a collection of storage cells together with associated circuits needed to transfer information in and out of storage. The memory stores binary information in groups of bits called words. A word in memory is an entity of bits that move in and out of storage as a unit. A memory word is a group of l's and O's and may represent a number, an instruction code, one or more alphanumeric characters, or any other binary-coded information. 
>A group of eight bits is called a byte.

> - `_The internal structure of a memory unit is specified by the number of words it contains and the number of bits in each word. Special input lines called address lines select one particular word. Each word in memory is assigned an identification number, called an address, starting from 0 and continuing with 1, 2, 3, up to 2' - 1 where k is the number of address lines. The selection of a specific word inside the memory is done by applying the k-bit binary address to the address lines. A decoder inside the memory accepts this address and opens the paths needed to select the bits of the specified word_`
