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

Does adjoining the xth roots of unity to the rational numbers, where x is any real number, produce the complex plane?
Related question: Does adjoining an open interval to the rational numbers generate the real numbers? The answer is yes, simply by translating the interval.
The answer to the first question is yes. Since if x is an element of the unit circle, its conjugate is also in the unit circle, we have that $x + \bar{x}$ is also in the field extension, and thus the line segment $[-1,1]$ is in the extension. This together with the fact that $i$ is a root of unity proves that the resulting field is the complex plane.

So any hope for continuous symmetries seems to be dead.

Long Term Goals:

Given a photo of an object at an angle possessing hidden bilateral symmetry, produce a texture that could be applied to a 3D model.
Obstructions:
- Normalizing the photo
- Detecting Symmetries
The first obstruction is resolved or at the very least half resolved. The problem arises from the 3D object being represented in the projective plane, and then being at an angle. Mathematically, we have maps $\mathbb{R}^3\to\mathbb{P}^2\to\mathbb{R}^2$ (an approximation, we also need to account for lens curvature and size). But there are already techniques that de-projectivize a photo into a projection from 3D space to a normal euclidean plane. The angle part could be solved by having a symmetry line.

Perhaps instead of using just irreducible polynomials in one variable, it would benefit to use homogeneous polynomials in two variables. Are they the analogue of single variable polynomials in the projective line?

Bibliography:
Infinite roots of unity: https://math.stackexchange.com/questions/1393072/adjoining-all-roots-of-unity-to-an-arbitrary-field-f-is-an-abelian-extension
