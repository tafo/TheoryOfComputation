# [Home](../README.md) 
## Definitions, Theorems and Proofs
* "Definitions" describe the objects and notions that we use
  * When defining some object we must make clear what constitutes that object and what does not
  * A definition assigns properties to some sort of mathematical object
    * For example, Euclid's Elements starts with a number of definitions, such as "a line is a breadthless length." After definitions, Euclid gives postulates or axioms. Based on these, he provides a number of proofs and constructions.
* After we have defined various objects and notions, we usually make mathematical "statements" about them
  * It must be precise. There must not be any ambiguity about its meaning
* A "proof" is a convincing logical argument that a statement is true
  * The explanation of why a statement is true
* A "theorem" is a mathematical statement proved true
  * A "lemma" is a true statement used in proving other true statements
    * A less important theorem that is helpful in the proof of other results
    * A short theorem used in proving a larger theorem
  * A "corollary" is a true statement that is a simple deduction from a thorem or proposition
    * A "proposition" is a less important but nonetheless interesting true statement
## Finding Proofs
* "P if and only if Q", often written "P iff Q", is designated as P &#8660; Q
  * The first part is "P only if Q", which means: If P is true, then Q is true, written P &#8658; Q
  * The second is "P if Q", which means: If Q is true, then P is true, written P &#8656; Q
  * The first of these parts is the "forward direction" of the original statement and the second is the "reverse direction"
  * To prove a statement of this form we must prove each of the two directions
    * Start with the easier one!
* Experimenting with examples is especially helpful
  * If the statement says that all objects of a certain type have a particular property, try to find a "counterexample"
    * The "counterexample" is an object that fails to have the property
    * If the statement actually is true, we will not be able to find a counterexample
    * This is a very general method in our algorithms!
* A well-written "proof" is a sequence of statements, wherein each one follows by simple reasoning from previous statements in the sequence
  * Some small details are left out where they are obvious e.g. the definition of "even" and "odd" numbers
* A few tips: be patient, come back to it, be neat, be concise
* Example: For any two sets A and B, (A &#8746; B)<sup>c</sup> = A<sup>c</sup> &#8745; B<sup>c</sup>
  * (This is one of DeMorgan's laws)
  * To prove this theorem we must show that the two sets (A &#8746; B)<sup>c</sup> and A<sup>c</sup> &#8745; B<sup>c</sup> are equal
  * Show that "every member of one set also is a member of the other and vice versa"
    * Suppose that x is an element of (A &#8746; B)<sup>c</sup>
    * Then x is not in A &#8746; B, from the definition of the complement of a set
    * Therefore x is not in A and x is not in B, from the definition of the union of two sets
    * In other words, x is in A<sup>c</sup> and x is in B<sup>c</sup>
    * Hence the definition of the intersection of two sets shows that x is in A<sup>c</sup> &#8745; B<sup>c</sup>
    * (For the other direction)
    * Suppose that x is A<sup>c</sup> &#8745; B<sup>c</sup>
    * Then x is in both A<sup>c</sup> &#8745; B<sup>c</sup>
    * Therefore x is not in A and x is not in B, and thus not in the union of these two sets
    * Hence x is in the complement of the union of these sets; in other words, x is in (A &#8746; B)<sup>c</sup> which completes the proof of the theorem
## Types of Proofs
#### Proof By Construction
Many theorems state that a particular type of object exists. One way to prove such a theorem is by demonstrating how to construct the object i.e. "proof by construction".

###### Theorem
For each even number n greater than 2, there exists a 3-regular graph with n nodes.

###### Proof
Let n be an even number greater than 2. Construct graph G = (N, E) with n nodes as follows.

The set of nodes of G is N = {0, 1, ..., n - 1}

The set of edges of G is E = { {i, i + 1} | for 0 &le; i &le; n - 2 } &#8746; { {n - 1, 0} } &#8746; { {i, i + n/2} | for 0 &le; i &le; n/2 - 1 }

Picture the nodes of this graph written consecutively around the circumference of a circle. In that case the edges described in the first and second subset of E go between adjacent pairs around the circle. The edges described in the third subset of E go between nodes on opposite sides of the circle. This mental picture clearly shows that every node in G has degree 3. 
