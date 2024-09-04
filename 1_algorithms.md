# Algorithms

## Instructions
You **do not** need a computer for today's tutorial. Your instructor will assign you to a group of 2-3. Introduce yourselves, then begin working on the following activities.

## Exercises
1. Otto the robot is not very smart.  In fact, his knowledge base includes only five instructions.  However, he can follow any sequence of instructions and does exactly what he is told, as long as they are known instructions.  He executes instructions in sequential order.

    Otto's knowledge base ("Otto language") consists of the following instructions:

    | Instruction                     | Details                                   |
    | ------------------------------- | ----------------------------------------- |
    | Stand up                        | must be sitting                           |
    | sit down                        | must be standing                          |
    | take a step                     | takes one step forward – must be standing |
    | turn                            | turns right 90 degrees – must be standing |
    | repeat x times  [ instruction ] | x must be a positive whole number         |

    Assumptions:
    - Otto starts in a **seated position**.
    - Otto must end in a seated position in the same chair.

    1. Write a sequence of instructions which direct Otto to walk forward five steps and then return to his resting state.

        > :stop_sign: Pause! Wait for further instructions.

    2. Write a sequence of instructions which direct Otto to walk in a square which is three steps on each side.  All turns are left-hand turns.

        > :stop_sign: Pause! Wait for further instructions.

2. In pseudocode, write an algorithm which reads a four-digit positive integer, and writes the number which is formed by placing the ones digit in the tens column and the thousands digit in the ones column. For example, if the input is 8052, the output is 28. If the input is 1234, the output is 41.

    You may assume the following arithmetic operations are available: +, –, ×, div and mod. "x div y" gives the whole quotient of x ÷ y, whereas "x mod y" gives the remainder.

3. Study the following algorithm, meant to run on a computer that can "read" inputs from some source, and "write" outputs to some destination. To see what it does, *trace* it (that is, follow it exactly step-by-step) using the input sequence: 7, 3, 8, 10, 4. Concisely but precisely, describe (a) its input, (b) its corresponding output and (c) it's purpose (the function it implements). Describe any assumptions made by the algorithm’s designer about the format of the input.

    ```
    read largest
    read number

    repeat until read was unsuccessful
        if number > largest
        then
            set largest = number

        read number

    write largest
    ```

    Note: it is assumed that the instruction `read var` attempts to read the next input value into variable var.  However, if there is no such value because the input is at an end (the input may be finite), then the latest read will be unsuccessful and var will contain an undefined value.  Assume also that it is always possible to ask if the most recent read was successful or not.

4. In pseudocode, design an algorithm which reads a sequence of one or more numbers, and determines how many of the numbers in the list are larger than the first.

5. Pretend that you are designing "Otto v2.0".
   1. Can you think of a useful modification to his current knowledge base, to shorten programs like the solution to 1a)?
   2. Re-write your solution to 1 b) for Otto 2.0 using your proposed modification.
   3. Can you suggest any other useful features to add to Otto v2.0's language?
   4. Otto lacks a decision making instruction.  Pretend that Otto v2.0 will be equipped with a proximity sensor.  This will enable him to sense whether or not he's too close to an object to take a step forward.  Design one or two instructions to add to his knowledge base so that an Otto programmer could make good use of them
   
6. In pseudocode, design an algorithm which will read three numbers and determine which is the largest and which is the smallest.
