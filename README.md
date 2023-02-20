# Galois Theory and Symmetries in Data

I used Sage 9.7 for the mathematical computations.
Finding symmetries in data is important in basically any branch of science. Group theory is essentially the study of symmetries. Galois theory is the study of
symmetries in the roots of polynomials. And polynomials are very simple functions with nice properties like being smooth. To that end, I will explore possible avenues 
of finding symmetries in data using Galois theory. Perhaps there will be some relationship with VCA at some point. 


Theoretical preamble:
The prerequisites for this is a solid understanding of basic Galois Theory, since I abuse definitions frequently. 
For example, the Galois group of a polynomial is only defined for the irreducible polynomials, but for reducible polynomials
one can simply say that it is the Galois group of the splitting field of the polynomial. A good reference for Galois theory is
Serge Lang's algebra, but Dummit and Foote will probably suffice since I won't be using any heavy theorems most likely.


Other than that, Profinite group theory might come into play at some point, and even then it might not suffice for continuous examples.
One can approximate a circle in the complex plane by the roots of unity. But the nth roots of unity are certainly not all the elements in the complex plane that have norm 1.
The nth roots of unity are countable by definition, but the elements with norm 1 are uncountable by virtue of being homeomorphic to the one point compactification of the real line. 
Perhaps there is a simpler reasoning to this, but that is the first thing I thought of.


Questions for the future:
Does adjoining the xth roots of unity to the rational numbers, where x is any real number, produce the complex plane?


Bibliography:
Infinite roots of unity: https://math.stackexchange.com/questions/1393072/adjoining-all-roots-of-unity-to-an-arbitrary-field-f-is-an-abelian-extension
