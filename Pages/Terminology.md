# [Home](../README.md) 
## Sets

* The objects in a set are called its elements or members
* We write 7 &#8712; {2,7,8} and 5 &#8713; {2,7,8}
  * {2,7,8} is a set
* A is a subset of B, written A &#8838; B, if every member of A also is a member of B
* A is a proper subset of B, written A &#8842; B, if A is a subset of B ant not equal to B
* If we do want to take the number of occurrences of members into account we call the group a "multiset" instead of a set
  * Thus, {7} and {7,7} are different as multisets but identical as sets
* We use "..." notation to denote a "infinite set". "..." notation means "continue the sequence forever"
  * Thus we write the set of "natural numbers" &#8469; as {1,2,3,...}
  * The set of integers &#8484; is written {...,-2,-1,0,2,2,...}
* The set with zero members is called the "empty set", written &#8709;
* When we want to describe a set containing elements according to some rule, we write {n | rule about n}
  * Thus {n | n = m&#0178; for some m &#8712; &#8469;} means the set of perfect squares
* The union of A and B is written A &#8746; B	
  * Combine all the elements in A and B into a single set
* The intersection of A and B is written A &#8745; B	
  * The set of elements that are in both A and B
* The complement of A, written A' or A<sup>c</sup>, is the set of all elements under consideration that are not in A
## Venn Diagram
* It represents sets as regions enclosed by circular lines
* Overlapping circles indicate common elements
  * Overlapping region is called intersection
* Check https://en.wikipedia.org/wiki/Venn_diagram 
## Sequences
* We usually designate a sequence by writing the list within parantheses
* The sequence 2,3,5 is written as (2,3,5)
* In a set, the order of elements doesn't matter. But, it is important in a sequence
  * Repetition does also matter in a sequence
* Finite sequences often are called "tuples"
  * A sequence with k elements is a k-tuple
  * A 2-tuple is also called a "pair"
    * The set of all pairs whose elements are 0s and 1s is {{0,0}, {0,1}, {1,0}, {1,1}}
* The "power set" of A is the all subsets of A
  * Thus if A is the set {0,1}, the power set of A is the set {&#8709;, 0, 1, {0,1}}
* If A and B are two sets, the "cartesian product" or "cross product" of A and B is written as "AxB"
  * "AxB" is the set of all pairs wherein "the first element &#8712; A" and "the second element &#8712; B"
  * Cartesian product of a set with itself is written as A&#8319;
    * A&#8319; = (n times) Ax...xA = {(a&#8321;, a&#8322;, ..., a&#8345;) | a&#7522; &#8712; A for every i &#8712; {1,...,n}}
    * It is also called as the "n-ary cartesian power" of A
## Functions and Relations
* A function is also called a mapping
  * if F(a) = b, we say that "F maps a to b"
* The set of possible inputs to a function is called its "domain"
* The outputs of a function come from a set called its "range"
  * Thus "F is a function with domain D and range R" denoted F : D &#8594; R
* A function F : X &#8594; Y is "onto" if there is an x(in X) for very y(in Y) such that F(x) = y
* The set of integers modulo n is written &#8484;&#8345; = {0, 1, ..., n-1}
* If the input to F is a k-tuple, we call it the "arguments" to F
  * A function with k arguments is called a "k-ary function", and k is called the "arity" of the function
  * If k is 1, F is then called a "unary" function
  * If k is 2, F is then called a "binary" function
    * Certain familiar binary functions are written in a special infix notation rather than in prefix notation
      * The addition function usually is written x+y, instead of add(x+y)
* A predicate is a function whose range is {TRUE, FALSE}
* A predicate whose domain is a set of k-tuples is called a k-ary relation
  * A 2-ary relation is called a binary relation
    * According to the set {Scissors, Paper, Stone} and relation beats
      * Scissors beat Paper, Paper beats Stone, Stone beats Scissors
    * A binary relation R is an "equivalence relation" if R is reflexive, symmetric and transitive
