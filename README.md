# BUILDING-PREFIX-INTERCHANGE-DISTANCE-DATABASE-FOR-SORTING-PERMUTATIONS-USING-PREFIX-BLOCK-INTERCHANG
Sorting by prefix block interchange is a combinatorial optimization problem in which a given permutation is to be sorted with minimum number of prefix block interchanges. The minimum number of prefix block interchanges required to sort a permutation is called the prefix block interchange distance of the permutation . The complexity class of this problem is unknown. As part of this project we build a database of prefix block interchange distances for permutations with length at most 7. Building such a database is useful in multiple ways. This could help understand the distribution of prefix block interchange distances, or it could help partition the symmetric group into various classes with same distance, or it could be used as a benchmark data for studying the optimality of various algorithms.
# BACKGROUND

The problem of transforming a given sequence into another using a specified set
of operations is a fundamental algorithmic problem that has received a lot of attention in the last decades dues to its multiple applications various fields such as
computational biology interconnection network design, and quantum computing.
The problem is formulated as follows. A permutation of n objects is a bijection
form the set to itself. The objects we consider are {1, 2, . . . , n}. The set of all permutations of these objects, along with function composition operation defines the
symmetric group Sn. A generating set of Sn, denoted by G is a subset of Sn such
that any permutation can be expressed as a finite composition of permutations in
G. A generating set is also called an operation.
Given two permutation, say α, β ∈ Sn and an operation G, the problem of
transforming α to β using the generators in G is a combinatorial optimization
problem that reduces to a sorting problem. A sequence of generators g1, g2. . . . gt
that transforms a given permutation to I is called a sorting sequence, where I
is the identity permutation in Sn. The problem that we study in this work is to
compute a shortest sequence of generators in G that sorts a given permutation π.
The length of shortest sequence is called the distance.
The problem is known to be NP-hard in general , but for some of operations,
it can be solved in polynomial time (e.g. block-interchanges and signed reversals ), while other families yield hard problems that admit good approximations
(e.g. 11/8 for reversals and for block-transpositions ).Several restrictions of these
families have also been studied, one of which stands out in the field of interconnection network design: the so-called prefix constraint, which forces operations
to act on a prefix of the permutation rather than on an arbitrary interval. Those restrictions were introduced as a way of reducing the size of the generated network
while maintaining a low value for its diameter, thereby guaranteeing a low maximum communication delay . The most famous example is perhaps the restriction
of reversals (which reverse the order of elements along an interval) to prefix reversals, and the corresponding problem known as pancake flipping, introduced
5
in and whose complexity was only settled thirty years later.
A permutation is an ordering/arrangement of elements in a set. For example,
consider a set S = {1,2,3}. The permutations are 123,132,213,231,312,321. For a set
containing n elements there are n! permutations. For example, the set S contains
3 elements and 3! = 6 permutations are there. We denote a permutation by the
symbol π. And a permutation along with the elements are generally represented
as π = π1 π2 π3 π4.... πi... πin where i is the index/position in the permutation.
