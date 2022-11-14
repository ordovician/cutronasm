# Calcutron-33 Assembly Support for VS Code

This is a plugin to help developing stuff in Calcutron-33 Assembly used by the made-up Calcutron-33 microprocessor, designed for teaching beginners to assembly programming. To get a quick introduction here is a simple program which reads a number N from input and writes to output every from N until 1. 

    // count down program
        loop:
        INP  x1     // load number to count down from
    decrement:
        OUT  x1     // write out counter to tape
        DEC  x1     // count down by one
        BGT  x1, x0, decrement
        JMP loop
        HLT

You use INP and OUT to handle I/O and HLT is used to stop execution of a program.