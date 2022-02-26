# push_swap

This is a project from the second circle of the 42cursus. (The best one i've done at the moment)

### Objectives :
  * Implement two stacks : 'stack a' and 'stack b'. (I used a linked list)
  * Put the numbers given as arguments in 'stack a' and then sort them using 'stack b' with the least amout of instructions possible.
  * Create a checker that checks if either your stack is sorted or not. (For the bonus part)

### Instructions to use
 * sa : swaps the first two elements of stack a
 * sb : swaps the first two elements of stack b 
 * ss : sa + sb
 * ra : shift all elements of stack a by one (the first element becomes the last)
 * rb : shift all elements of stack b by one (the first element becomes the last)
 * rr : ra + rb
 * rra : shift down all elements of stack a by one (the last element becomes the first)
 * rrb : shift down all elements of stack b by one (the last element becomes the first)
 * rrr : rra + rrb
 * pa : push the first element in stack b to stack a
 * pb : push the first element in stack a to stack b

### Skills I learnt from it :
  * Some sorting algorithms
  * Problem solving, AI
  * Unix
    
### Final grade :
  125/100.

### Number of instructions to sort a stack :
 * For 100 numbers : instructions < 700.
 * For 500 numbers : instructions < 5500.


### How to use
  1. Clone and type make in the terminal, then type './push_swap ' with the numbers you want to sort, it will return the instructions to sort them in a stack.
  2. If you want to check the number of instructions, use the command 'wc' with the option 'l'. Example (./push_swap 5 2 3 1 7 | wc -l).
  3. For the checker, it must be ready after typing make. If executed alone it will wait for the instructions in the standard input, else, execute it with the arguments given in a stack using a pipe, it will return 'OK' if the stack is sorted and 'KO' if not. (example './push_swap ARGS | ./checker ARGS')
