# [Home](../README.md) 
## FINITE AUTOMATA(FINITE-STATE MACHINE)
A **finite-state machine(FSM)** or **finite-state automaton(FSA**, plural: automata), finite automaton, or simply a **state machine**, is a mathematical model of computation used to recognize patterns. It is an abstract machine that can be in exactly one of a finite number of **states** at any given time. It can change from one state to another in response to some inputs; the change from one state to another is called a **transition**. At the time of transition, the automata can either move to the next state or stay in the same state. The automaton processes the input(string of symbols) and produces an output. The output is either **accept** or **reject**. When it reads the last symbol, it produces its output. The output is *accept* if it is in **accept state** and *reject* if it is in **reject state**. 

#### FORMAL DEFINITION OF FINITE AUTOMATA
A finite automaton is a 5-tuple (Q, &#8721;, &#0948;, q&#8320;, F), where:
* Q is a finite set called the **states**
* &#8721; is a finite set called the **alphabet(the set of input symbols)**
* &#0948;: Q x &#8721; &#8594; Q is the **transition function**
* q&#8320; &#8712; Q is the **start(initial) state**
* F &#8838; Q is the **final states(set of accept states)**
