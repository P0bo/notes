# LEC 01 - Natural Numbers and their Operations

## Division and factors

- a divides b if b mod a is 0
  - a | b
  - b is a multiple of a 
- a is a factor of b if a | b
- factors occur in pairs -- factors of 13 are 
  - {1, 12}, {2, 6}, {3, 4}
- ...unless the number is a perfect square --
  - factors of 36 :
  - {1, 36}, {2, 18}, {3, 12}, {4, 9}, {6}

## Prime Numbers

- p is a prime if it only has two factors {1, p}
  - 1 is not a prime -- only one factor

- Prime numbers are 2, 3, 5, 7, 11, 13
  - Sieve of Eratosthenes -- remove multiples of p 
- Every number can be decomposed into prime factors 
  - 12 = 2 * 2 * 3 =$2^2$ * 3
  - 126 = 2 * 3 * 3 * 7 = 2 * $3^2$ * 7
- This decomposition is unique -- prime factorisation

## Summery

- N - Natural numbers {0,1,2,3,4...}
- Z - Integers {..., 3, 2, 1, 0, 1, 2, 3, ...}
- Arithmatic Operations: +, -, *, /, $m^n$
- Divisibility, a | b
- Factors
- Prime Numbers

# LEC 02 - Rational Number

## Division

- Can't represent 19/5 as an integer
- Fractions 3+4/5
- Rational number: p/q, p and q are integer
  - Numerator p, denominator q, q != 0
  - Use Q to denote rational numbers

- The same number can be written in many ways
  - 3/5 = 6/10 = 30/50
- Usefull to add, substract, compare rationals
  - 3/5 + 3/4 = 12/20 + 15/20 = 27/20
  - 3/5 < 3/4 because 12/20 < 15/20

- The most basic form of a fraction is p/q; where p,q have no common factors
  - Reduced form of 18/60 is 3/10

- Greatest Common Divisor : gcd(18, 60) = 6
  - Recal prime factorisation
  - 18 = 2 * 3 * 3, 60 = 2 * 2 * 3 * 5
  - Common prime factors are 2 * 3
  - Can find gcd(m,n) more efficiently

## Density

- For each integer, we have a next integer and a previous integer
  - For m, next is m + 1, previous is m - 1
  - Next: No integer between m and m + 1 
  - Previous: No integer between m and m - 1
- Between two rationals we can alwys find another one
  - Suppose m/n < p/q
    - Their average (m/n + p/q)/2 alwys lies between them
- Rationals are Dense, integers are Discrete

## Summery

- Q: rational numbers
- p/q, where p,q are integers
- Representaion is not unique
  - p/q = (n * p)/(n * q)
- Rationals are dense, we can't talk about previous or next

# LEC 03 - Real and Complex numbers

## Beyond rationls 

- Rationls are dense 
  - Between any two rationals we can always find another one 
- Is evry point on the number line a rational number?
- For a integer m, its a square is m^2 = m * m 
- Square root of m, $\sqrt{m}$, r such that r * r = m
- Perfect Squares -- 1,4,9,16,25,...,256,...
- What about integers that are not perfect squares?
- $\sqrt{2}$ can't be written as p/q 
- Yet we can draw a line of length $\sqrt{2}$
  - Diagonal of a square whose sides have length 1
- $\sqrt{2}$ is Irrational Number
- Proper numbers: R -- all rational and irrational numbers 
- Like raionals, real numbers are dense 
  - If r < r', then (r + r')/2} lies between r and r'
- Some well known irrational numbers 
  - $\pi$ = 3.1415927...
  - $e$ = 2.7182818...

## Beyond Real numbers

- Can we stop with real numbers?
  - What about $\sqrt{-1}$
  - For any real number r, $r^2$ must be positive -- law of signs for multiplication
- $\sqrt{-1}$ is a Complex Number 

## Summery
- Real numbers extend rational numbers
- Typical irrational numbers -- square roots of integers that are not perfect square
- Real Numbers are dense, like rationls 
- Evert Natural number is an integer
- Every integer is a Rational Number
- Every Rational number is a Real number
- Complex numbers extend real numbers

# LEC 04 - Set Theory

## Sets

- A set is a collection of items 
  - Days of the weel:
  - {Sun, Mon, Tue, Wed, Thu, Fri, Sat}
- Factors of 24:
  - {1,2,3,4,6,8,12,24}
- Primes below 15:
  - {2,3,5,7,11,13}
- Sets may be infinite 
  - Differnt types of numbers: N, Z, Q, R
- No requirement that members of a set have uniform type
  - Set of objects of a painting

## Order, duplicates, cardinality

- Sets are unordered 
  - {Kohli, Dhoni, Pujars}
  - {Pujara, Dhoni, Kohli}
- Duplicates don't matter
  - {Kohli, Dhoni, Pujara, Kohli}
- Cardinality: number of items in a set
  - for finite sets, count the items 
    - {1,2,3,4,6,8,12,24}
    - May not be obvious that a set is finite
  - What abot infinite sets?
    - is Q bigger than Z?
    - is R bigger than Q?

## Describe sets, membership

- Finite sets can be listed out explicitly
  - {Kohli, Dhoni, Pujara}
  - {1,2,3,4,6,8,12,24}
- Infinite sets can't be listed out 
  - N = {0,1,2,...} is not a formal notation
- Not every collection of items is a set
  - Collection of all sets is not a set 
  - Russel's Paradox: Seperate discussion
- Items in a set are called elements
  - Membership: $x \in X$, x is an element of X
  - $5 \in Z$, $\sqrt{2} \notin Q$

## Subsets

- X is a subset of Y
  - Every element of X is also an element of Y
- Notation: $X \subseteq Y$
- Examples 
  - {Kohli, Pujara} \subseteq {Kohli, Pujara, Dhoni}
  - $Primes \subseteq N$, $N \subseteq Z$, $Z \subseteq Q$, $Q \subseteq R$
- Every set is a subset of itself : X \subseteq Y
  - X = Y if and only if $X \subseteq Y$ and $Y \subseteq X$
- Proper subset: $X \subseteq Y$ but X != Y
  - Notation: $X \nsubseteq Y$
  - $N \nsubseteq Z$, $Z \nsubseteq Q$, $Q \nsubseteq R$

## The empty set and the powerset

-  The empty set has no element -- \emptyset
- $\emptyset \subseteq X$ for every set X
  - Every element of $\emptyset$ is also in X
- A set can also contain sets
- Powerset set of subsets of a set
  - X = {a, b}
  - Powerset is {$\emptyset$, {a}, {b}, {a, b}}
    - Powerset of $\emptyset$ is {$\emptyset$}
- Set with n elements has $2^n$ subsets
  - X = {$X_1$,$X_1$,...$X_n$}
  - In a subset, either include of exclude each $x_i$
  - 2 Choices per element 2 * 2 * ... 2 = $2^n$

### Subsets and binary numbers 

- X = {$X_1$,$X_1$,...$X_n$}
- n bit binary numbers 
  - 3 bits: 000, 001, 010, 011, 100, 101, 110, 111
- Digit $i$ represents wheather $X_i$ is included in a subset
  - X = {a, b, c, d}
  - 0101 is {b, d}
  - 0000 is $\emptyset$, 1111 is X

# LEC 05 - Construction of Subsets and set Operations

## Constructing subsets

### Set comprehension

- The subset of even integers 
{$X | X \in \mathbb{Z}, x mod 2 = 0$}
    - Begin with an existing  set, $\mathbb{Z}$
    - Apply a condition to each element in that set 
      - $ x \in \mathbb{Z}$ such that x mod 2 = 0)
      - Collect all the elements that match the condition
- Examples
  - The set of perfect squares
  {$m | m \in \mathbb{N},\sqrt{m} \in \mathbb{N}$}
  - The set of rationals in reduced form
  {$p/q | p, q \in \mathbb{X}, gcd(p,q) = 1$}

### Intervals 

- Integers from -6 to +6 
{$z | z \in \mathbb{X},-6 \leq z \leq +6$}
- Real numbers between 0 and 1
  - Closed interval $[0, 1]$
    - Include endpoints
    {$r | r \in \mathbb{R}, 0 \leq r \leq 1$}
  - Open interval (0,1)
    - Exclude endpoints
    {$r | r \in \mathbb{R}, 0 < r < 1$}
  - Mixed 
    - Left open (0,1]
    {$r | r \in \mathbb{R}, 0 < r \leq 1$}
    - Right open [0,1)
    {$r | r \in \mathbb{R}, 0 \leq r < 1$}

## Union, intersection, complement

- Union -- combine X and Y, $X \cup Y$
{a, b, c} $\cup$ {c, d, e} = {a, b, c, d, e}
- Intersection -- elements common to X and Y 
{a, b, c, d} $\cap$ {a, d, e, f} = {a, d}
- Set difference -- elements in X hat are not common to Y, X/Y or X - Y
{a, b, c, d}\{a, d, e, f} = {b, c}
- Complement -- elements not in X, $X^c$ or $X^{\prime}$
  - Define complement relative to larger set, universe
  - Complement of prime numbers in $\mathbb{N}$ are composite numbers

## Summery
- Sets are standard way to represent collections of mathematical objects 
- Sets may be finite or infinite 
- Can carve out interesting subsets of ssets 
- Set operations: union, intersectiom, difference, complement

# LEC 06 - Sets Example

## Sets

- A set is collection of items 
- Finite sets can be listed out explicitly
  - {Kohli, Dhoni, Pujara}, {1, 4, 9, 16, 25}
- Infinite sets can't be listed out
  - $\mathbb{Z} = \{..., -2, -1, 0, 1, 2, ...\}$
- $Membership x \in X, Subset X \subseteq Y$
  - 5 $\in$ $\mathbb{Z}$, $\sqrt{2}$ $\notin$ $\mathbb{Q}$
  - $Primes \subseteq \mathbb{N}, \mathbb{N}\subseteq \mathbb{Z}, \mathbb{Z} \subseteq \mathbb{Q}, \mathbb{Q},\subseteq \mathbb{R}$
- Powerset -- set of subsets of a set 
  - X = {a, b}, powerset $\{\emptyset, \{a\}, \{b\}, \{a, b\}\}$
  - Set with n elements has $2^n$ subsets

## Set comprehension 

- Squares of even integers
  - $\{x^2 | x \in \mathbb{Z}, x\ mod\ 2\ =\ 0\}$
    - Generate Elements drawn from existing set
    - filter Select Elements that satisfyy a constraint
    - Transform Modify selected elements
- More filters 
  - Rationals in reduced form
    - $\{p/q\ |\ p/q\ \in\ \mathbb{Q},\ gcd(p,q)\ =\ 1\}$
  - Reals in interval [-1, 2)
    - $\{r\ |\ r\ \in \mathbb{R},\ -1\ \le\ r\ <\ 2\}$
  - Cubes of first 5 natural numbers 
    - Y = $\{n^3 | n \in \{0,\ 1,\ 2,\ 3,\ 4\}\}$
  - Cubes of first 500 natural numbers ?
    - Y = $\{n^3 | n \in \{0,\ 1,\ 2,\ 3,\ 4,\ ...\ 498,\ 499\}\}$
  - Use a set comprehension to define first 500 natural numbers 
    - X = $\{n\ |\ n\ \in\ \mathbb{N},\ n\ <\ 500\}$
  - Now, a more readable version
    - X = $\{n\ |\ n\ \in\ \mathbb{N},\ n\ <\ 500\}$
    - Y $\{n^3\ |\ n\ \in\ X\}$
- Perfect squares
  - Integers whose square root is also an integer
    - $\{z\ |\ z\ \in \mathbb{Z},\ \sqrt{z}\ \in\ \mathbb{Z}\}$
  - All squares are positive, so this is the same as
    - $\{x\ |\ x\ \in \mathbb{N},\ \sqrt{n}\ \in\ \mathbb{N}\}$
  - Alternatively, generate all the perfect squares
    - $\{n^2\ |\ n\ \in\ \mathbb{N}\}$
  - Extend the defination to rationals
    - $\frac{9}{16} = {(\frac{3}{4})}^2$ is a square, $\frac{1}{2} \ne {(\frac{p}{q})}^2$ for any p,q
    - $\{\ q\ |\ q\ \in\ \mathbb{Q},\ \sqrt{q}\ \in\ \mathbb{Q}\}$ or $\{q^2\ |\ \in\ \mathbb{Q}\}$
  - Choose the generator as required 

# LEC 07 - Examples of Set Operations and Counting Problems

## Counting Problems

- In a class, 30 students took Physics, 25 took Biology and 10 took both, and 5 took neither, How many students are there in the class?
  - Draw sets of for Physics(P) and Biology(B) 
  - 10 students are in $P \cap B$
  - This leaves 20 students in P \ B , took Physics but not Biology
  - Likewise 15 students in B \ P , tool Biology but not Physics
  - 5 students in $\overline{P \cup B}$ in the class, but neither took Physics nor Biology 
- Class strength: 5 + 20 + 10 + 15 = 50

- In a class of 55 students, 32 took Physics, 11 took both Physics and Biology, and 7 tool neither.  how many students took Biology but not Physics ?
  - 21 + 7 + x + 11 =55
  - x = 55 - 39 
  - x = 16 

- In a class of 60 students, 35 took Physics,30 tool Biology, and 10 took neither. How many took both Physics  and Biology?
  - $|Y|$ : Cardinality of Y (number of elements)
  - $|P| + |B|$ = 35 + 30 = 65
  - $|P \cup B|$ = 60 - 10 =  50 
  - So the students who have taken both must be 65 - 50 = 15

## Summery

- Set notation is useful way to concisely describe collections of objects
- Set comprehension combines generators, filters and transformers to produce new sets from old 
- Venn diagrams can be useful to work out problems involving Sets

# LEC 08 - Relations

## New sets from old sets 

- A set is a collection of items 
- We can combine sets to form new ones 
  - $X\ \cup\ Y,\ X\ \cap\ Y,$ $X$ \ $Y$
  - $\overline{X}$ with respect to $Y$
- Define subsets using set comprehension
  - Odd integers
    - $\{z\ |\ z \in\ \mathbb{Z},\ z\ mod\ 2=1\}$
  - Rationals not in reduced form
    - $\{p/q|\ p,q\in\mathbb{Z},gcd(p,q)>1\}$
  - Reals in [3, 17)
    - $\{r|r\in\mathbb{R},3\le17\}$

## Cartesian product

- $A\times B=\{(a,b)|a\in A,b\in B\}$
  - Pair up elements from A and B 
  - A = {0, 1}, B = {2,3}
  - $A\times B= \{(0,2),(0,3),(1,2),(1,3)\}$
- In a pair, the order is important 
  - $(0,1)\ne(1,0)$
- For sets of numbers, visualize product as two dimentional space 
  - $\mathbb{N}\times\mathbb{N}$
  - $\mathbb{R}\times\mathbb{R}$

## Binary Relations

- Select some pairs from the Cartesian product
- Combine Cartesian product with set comprehension 
- $\{(m,n)|(m,n)\in\mathbb{N}\times\mathbb{N},n = m+1\}$
  - {(0,1),(1,2),(2,3),...,(17,18),...}
- Pairs (d,n) where d is a factor if n 
  - $\{(d,n)|(d,n)\in\mathbb{N}\times\mathbb{N},d|n\}$
  - $\{(1,1),...,(2,82),...,(14,56),...\}$
- $Binary\ Relation R \sube A\times B$
- Notation: $(a,b)\in R\ or\ aRb$

### More relations

- Teachers and courses
  - T, set of teachers in a college
  - C, set of courses being offered 
  - $A\sube T\times C$ describes the allocation of teachers to course
  - $A = \{(t,c)|(t,c)\in T\times C, t\ teaches\ c\}$
- Mother and child
  - P, set of people in a country
  - M $\sube$ P $\times$ P relates mothers to children
  - $M= \{(m,c)|(m,c)\in P\times P, m\ is\ the\ mother\ of\ c\}$
- Points at a distence 5 from (0,0)
  - Distance from (0,0) to (a,b) is $\sqrt{a^2+b^2}$
  - $\{(a,b)|(a,b)\in\mathbb{R}\times\mathbb{R},\sqrt{a^2+b^2}=5\}$
  - $\{(0,5),(5,0),(3,4),(-3,-4),...\}$
- Rationals in reduced form 
  - A subset Q
    - $\{p/q|(p,q)\in\mathbb{Z}\times\mathbb{Z},gcd(p,q)=1\}$
  - ... But we can also think of it as
    - $\{(p,q)|(p,q)\in\mathbb{Z}\times\mathbb{Z},gcd(p,q)=1\}$

## Beyond binary realtions

- Cartesian products of more than two sets
- Pythagorean triples
  - Square on the hypotenuse is the sum of the squares on the oposite sides
  - $\{(a,b,c|(a,b,c)\in\mathbb{N}\times\mathbb{N}\times\mathbb{N},a,b,c>0,a^2+b^2=c^2\}$
- Corners squares
  - A corner is a point $(x,y)\in\mathbb{R}\times\mathbb{R}$
  - $((x_1,y_1),(x_2,y_2),(x_3,y_3),(x_4,y_4))$ are related if they are the corner of a square
  - For instance
    - $((0,0),(0,2),(2,2),(2,0))$
    - $((0.5,0),(0,0.5),(0.5,1),(1,0.5)$
  - $Sq\sub{\mathbb{R}}^2\times{\mathbb{R}}^2\times{\mathbb{R}}^2\times{\mathbb{R}}^2$

## Back to BInary Relations

- Identity relation $I\sube A\times A$
  - I = $\{(a,b)|(a,b)\in A\times A, a=b\}$
  - I = $\{(a,a)|(a,a)\in A\times A\}$
  - I = $\{(a,a)|a\in A\}$
- Reflexive relations
  - $R\sube A\times A, I\sube R$
  - $\{(a,b)|(a,b)\in\mathbb{N},a,b>0,a|b\}$
    - $a|a$ for all $a > 0$
- Symmetric relations
  - $(a,b)\in R$ if and only if $(b,a)\in R$
  - $\{(a,b)|(a,b)\in\mathbb{N}\times\mathbb{N},gcd(a,b)=1\}$
  - $\{(a,b)|(a,b)\in\mathbb{N}\times\mathbb{N},|a-b|=2\}$
- Transitive relations
  - If $(a,b)\in R$ and $(b,c)\in R$ then $(a,c) \in R$
  - $\{(a,b)|(a,b)\in\mathbb{N}\times\mathbb{N},a|b\}$
    - If $a|b$ and $b|c$ them $a|c$
  - $\{(a,b)|(a,b)\in\mathbb{R}\times\mathbb{R},a<b\}$
    - If $a<b$ and $b<c$ then $a<c$
- AntiSymmetric relations
  - If $(a,b)\in R\ and\ a \neq b,\ then\ (b,a) \notin R$\
    - If $a<b$ then $b\nless a$
  - $M\sube P\times P$ relates mothers to children 
    - If $(p,c)\in M\ then\ (c,p)\notin M$

## Equivalence relations

- Reflexive, Symmetric and Transitive
- Same remainder modulo 5 
  - 7 mod 5 = 2, 22 mod 5 = 2 
  - If a mod 5 = b mod 5 then (b - a) is a multiple of 5 
  - $\mathbb{Z}mod 5 = \{(a,b)|a,b\in\mathbb{Z},(b-a)\ mod\ 5=0\}$
  - Divides integers into 5 groups based on remainder when divided by 5 
- An equivalence relation partitions a set 
- Groups of equivalent elements are called equivalence classes

## Summery 

- Cartesian products generate n-tuples from n sets 
  - $(x_1,x_2,...,X_n)\in X_1\times X_2\times...\times X_n$
- A relation picks out a subset of a Cartesian product
  - $\{(m,r)|(m,r)\in\mathbb{N}\times\mathbb{R},r=\sqrt{m}\}$
- Properties of Relations
  - Reflexive, Symmetric, Transitive, AntiSymmetric
- Equivalence relations partition a set

# LEC 09 - Functions

- A rule to map inputs to outputs
- Convert $x\ to\ x^2$
  - The rule: $x\to x^2$
  - Give it a name: $sq(x)=x^2$
    - Input is a parameter 


<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Y%3Dx%5E2.svg/1200px-Y%3Dx%5E2.svg.png" style="background-color:#bbb;border-radius:10px;margin:0 0 10px 0;">

- Need to specify the Input and output sets
- Domain: Input set
- $domain(sq) = \mathbb{R}$
- Codomain: Output set of possibles
- $codomain(sq)=\mathbb{R}$
- Range: Actual values that the output can take 
- $range(sq)=\mathbb{R}\geq=\{r|r\in\mathbb{R},r\geq0\}$
- $f:X\to Y$, domain of $f$ is $X$, codomain is $Y$

## Functions and Relations

- Associate a relation $R_f$ with each function $f$
- $R_{sq}=\{(x,y)|x,y\in\mathbb{R}, y = x^2\}$
- Additonal notation: $y = x^2$
- $R_f\sub domain(f)\times range(f)$
- Properties of $R_f$
- Defined on the entire domain
- For each $x\in domain(f)$, there is a pair $(x,y)\in R_f$
- Single-valued
- For each $x\in domain(f)$, there is exactly one $y\in codomain(f)$ such that $(x,y)\in R_f$
- Drawing $f$ as a graph is plotting $R_f$

## Lines

- <text style="color:#f55">$f(x)=3.5x+5.7$
- 3.5 is the slope
- 5.7 is intercept where the line crosses the y axis when $x=0$
- Changing the slope and intercept produce differnt lines
- <text style="color:#29f">$f(x)=2x+5.7$
- <text style="color:#5f5">$f(x)=-4.5x+2.5$

<div style="position: relative; width: 100%; padding-bottom: 100%; height: 0">
<iframe 
        src="https://www.desmos.com/calculator/bvjhaqn93p?embed"
        style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 1px solid #ccc;border-radius:10px;margin:0 0 10px 0;"
        frameborder="0"
    ></iframe>
</div>
<br>

## More functions 

- $x\to \sqrt{x}$
- Is this a function ?
- <text style="color:#f55">$5^2=(-5)^2=25$
- By convention,take positive square root

<div style="position: relative; width: 100%; padding-bottom: 100%; height: 0">
<iframe 
        src="https://www.desmos.com/calculator/9s1pqdkrcp?embed"
        style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 1px solid #ccc;border-radius:10px;margin:0 0 10px 0;"
        frameborder="0"
    ></iframe>
</div>
<br>

- What is the domain?
- Depends on the codomain
- Negative numbers do not have real square roots
- If codomain is $\mathbb{R}$, domain is $\mathbb{R}\ge 0$
- If codomain is the set $\mathbb{C}$ of complex numbers, domain is $\mathbb{R}$

## Types of function

- $Injective$: Differnt inputs produces differnt outputs $\to$ one-to-one
- If $x_1\ne x_2,f(x_1)\ne f(x_2)$
- <text style="color:#f55">$f(x)=3x+5$ is $Injective$
- <text style="color:#59f">$f(x)=7x^2$ is not; for any $a, f(a)=f(-a)$ 

<div style="position: relative; width: 100%; padding-bottom: 100%; height: 0">
<iframe 
        src="https://www.desmos.com/calculator/mm7a0pxgen?embed"
        style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 1px solid #ccc;border-radius:10px;margin:0 0 10px 0;"
        frameborder="0"
    ></iframe>
</div>
<br>

- $Surjective$: Range is the codomain $\to$ onto
- For every $y\in codomain(f)$, there's an $x\in domain(f)$ such that $f(x)=y$
- <text style="color:#f25">$f(x)=-7x+10$ is Surjective
- <text style="color:#29f">$f(x)=5x^2+3$ id not surjective for codomain $\mathbb{R}$
- <text style="color:#5f5">$f(x) = 7\sqrt{x}$ is not surjective for codomain $\mathbb{R}$

<div style="position: relative; width: 100%; padding-bottom: 100%; height: 0">
    <iframe 
        src="https://www.desmos.com/calculator/ielw95tlbk?embed"
        style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 1px solid #ccc;border-radius:10px;margin:0 0 10px 0;"
        frameborder="0"
    ></iframe>
</div>
<br>

## Properties of functions

- $Bijective:1\to1$ correspondence between domain and Codomain
- Every $x\in domain(f)$ maps to a distinct $y\in codomain(f)$
- Every $y\in codomain(f)$ has a unique pre-image $x\in domain(f)$ such that $y=f(x)$
<br>
<center>

| Theorem |
| ------------- |
| A function is bijective if and only if it is Injective and Surjective |
</center>

- From defination, if a function is bijective then it is injective and surjective 
- Suppose a function $f$ is injective and surjective 
- Injectivity guarantees that $f$ satisfies the first condition of a bijection.
- Surjectivity says every $y\in codomain(f)$ has pre-image. Injectivity guarantees this pre-image is unique

### Bijections and Cardinality 

- For finite sets we can count the items 
- What if we have two large sacks filled with marbles?
- Do we need to count the marbles in each sack?
- Pull out parbles in pairs, one from each sack
- Do both sacks become empty simultaneously?
- Bijection between the marbles in the sacks
- For infinite sets
- Number if lines is the same as  $\mathbb{R}\times\mathbb{R}$
- Every line $y=mx+c$ is determined by by (m,c) and vice versa
- For every pair of points $(x_1,y_1)\ and\ (x_2,y_2)$ there is a unique line passing through both points
- Number of lines is the same as cardinality of $\mathbb{R}\times\mathbb{R}$
- Does this show that $(\mathbb{R}\times\mathbb{R})\times(\mathbb{R}\times\mathbb{R})=\mathbb{R}^2\times\mathbb{R}^2$
- The correspondence is $not\ Bijection$ -- many pairs of points describe the same line
- Be careful to establish that a function is a bijection 

## Summery

- A function is given by rule mapping inputs to outputs
- Define the domain, codomain and range
- Associate a relation $R_f$ with each function $f$
- Properties of functions: injective (one-to-one),surjective (onto)
- Bijections: injective and surjective (one-to-one and onto)
- A bijection establishes that domain and codomain have same cardinality

# LEC 10 - Relations: Examples

## Relations 

- $A\times B$ --- Cartesian product, all pairs $(a,b),a\in A\ and\ b\in B$
- A = {x, y, z}, B = {p, q, r}
$$
A\times B= \{(x,p),(x,q),(x,r),(y,p),(y,q),(y,r),(z,p),(z,q),(z,r)\}\\
B\times A= \{(p,x),(p,y),(p,z),(q,x),(q,y),(q,z),(r,x),(r,y),(r,z)\}
$$
- We can take Cartesian product of more than two sets 
$$
A\times B = \{(x,p,x),(x,p,y),(x,p,z),(x,q,x),(x,q,y),...,(z,r,x),(z,r,y),(z,r,z)\}
$$
- A relation picks out certain tuples in the Cartesian product
- Let $A = \{1,4,7\},B= \{1,16,49\}$
- $S\sube A\times B = {(1,1),(4,16),(7,49)}$
- $S= \{(a,b)|(a,b)\in A\times B,b=a^2\}$

## Examples of relations

- Divisibility 
- Pairs of natural numbers (d, n) such that d|n ($d\ mod\ n=0$)
- Pairs such as (7,63),(17,85),(3,9),...
- $D=\{(d,n)|(d,n)\in\mathbb{N}\times\mathbb{N}\}$
- Can also extend to integer divisors
- $E = \{(d,n)|(d,,n)\in \mathbb{Z}\times\mathbb{N},d|n\}$
- Now (-7,63),(-17,85),(-3,9),... are also in E
- Prime power
- Pairs of natural numbers $(p,n)$ such that $p$ is prime and $n = p^m$ for some natural number $m$ 
- Examples: (3,1),(5,625),(7,343),...
- First define primes: $P=\{p|p\in\mathbb{N},factors(p)=\{1,p\},p\ne1\}$
- Prime powers: $PP=\{(p,n)|(p,n)\in P\times\mathbb{N},n=p^m\ for\ some\ m\in\mathbb{N}\}$

## Beyond numbers 

### Tables as relations

- Airline routes
- An airline flies to set cities --- e.g. Bangalore, Chennai, Delhi, Kolkata
- Let $C$ denote the set of cities served by the airline 
- Some cities are connected by direct flights
- $D\sub C \times C$
- Is $D$ reflexive, irreflexive?
- Hopefully irreflexive!
- Is $D$ symmetric? 
- If there's a direct flight from Bangalore to Delhi, is there always a direct flight back from Delhi to Bangalore?
- For bigger cities, maybe yes
- For smaller cities, may have a triangular route
$$
Chennai\to Madurai\to Salem\to Chennai
$$
- - Flying distances between cities
<center>

| Source | Destination | Distance(km) |
| --------------- | --------------- | --------------- |
| Bangalore | Chennai | 290 |
| Chennai | Delhi | 1752 |
| Delhi | Bangalore | 1735 |
| Delhi | Chennai | 1752 |
|...|...|...|

</center>

- - - Table is a relation: $Dist\sube C\times C\times \mathbb{N}$
- Some entries are useless: (Delhi, Delhi, 0)
- $Dist=\{(a,b,d)|(a,b)\in D,d\ is\ distance\ from\ a\ to\ b\}$
- Distances are symmetric, even if $D$ is not
- Save space by representing only one direction in the table 
- - Student table
<center><table>
<tr><th>Student Table</th><th>Marks Table</th></tr>
    <tr><td>

| Roll No | Name | Date of Birth |
| --------------- | --------------- | --------------- |
| A3456 | Abhay Singh | 03-07-2001 |
| B4567 | Payel Ghosh | 18-06-1999 |
| F4567 | Jeremy Pinto | 22-02-2000 |
| C9876 | Payal Ghosh | 14-05-2000 |
|...|...|...|

 </td><td>

| Roll No | Subject | Grade |
| --------------- | --------------- | --------------- |
| A3456 | English | B |
| B4567 | Mathematics | A |
| F4567 | Physics | B |
| C9876 | Chemistry | A |
|...|...|...|

</td></tr>
</table>
</center>

- - Generate a table with roll numbers, names and grades
- Join the ralations on Roll No 
- $\{(r,n,s,g)|(r,n,d)\in Students,(r,s,g)\in Grades,r = r\}$
<center>

| Roll No | Name | Subject | Grade |
| --------------- | --------------- | --------------- | --------------- |
| A3456 | Abhay Singh | English | B |
| B4567 | Payel Ghosh | Mathematics | A |
| F4567 | Jeremy Pinto | Physics | B |
| C9876 | Payel Ghosh | Chemistry | A |


</center>

## Summery

- A relation describes special tuples in Cartesian product
- Data tables are essentially relations 
- Combining information on tables on tables can be described in terms of operations on relations

# LEC 11 - Functions: Examples

## Functions

- A rule to map inputs to outputs
  - $X\to x^2,g(x)=x^2$
- Domain, codomain, range
- Associated relation
  - $R{sq}=\{x,y|x,y\in\mathbb{R},y=x^2\}$
- Can have functions on ther sets
  - $Mother:People\to People$
- We will focus more on functions on numbers
- What question are we interested in ?

### Range of values

- What range of values does the output span?
- <text style="color:#f55">$f(x)=x^2$ is always positive to the rangle is 0 to $+\infty$
- <text style="color:#2af">$f(x)=x^3-3x^2+5$ ranges from $-\infty$ to $+\infty$
- <text style="color:#5f5">$f(x)=5sin(x)$ has bounded range, from $-5$ to $+5$

<div style="position: relative; width: 100%; padding-bottom: 50%; height: 0">
    <iframe 
        src="https://www.desmos.com/calculator/eqmh7ptwn6?embed"
        style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 1px solid #ccc;border-radius:10px;margin:0 0 10px 0;"
        frameborder="0"
    ></iframe>
</div>
<br>

### Maxima and Minima

- $f(x)=x^2$ attains a minimum value at $x=0$, no maximum vlaue
- $f(x)= x^3-3x^2+5$ has no global minimum or maximum, but a $local\ maximum$ at $x=0$ and $local\ minimum$ at $x=2$
- $f(x)=5sin(x)$ periodically attains minimum and maximum value $-5$ and $+5$, infinitely often

### Comparing Functions

- Does one function grow faster than another?
- $f(x) = x^3+3x^2+5$ grows faster than $g(x)=x^2$
- Let $G(y)$ be the number of Data Science graduates in year y 
- Let $J(y)$ be the number of new Data Science jobs in year y 
- Ideally, $G(y)$ and $J(y)$ should grow at similar retes 
- If $J(y)$ grows faster than $G(y)$, more students will opt to study Data Science

## Summery

- We will typically study functions over numbers 
- Many properties of functions are interesting
  - Range of ooutputs 
  - Inputs for which function attains (local) maximum, minimum value 
  - Relative growth rates of functions

# LEC 12 - Prime Numbers 

## How many prime numbers are there?

- A prome number $p$ has exactly two factors, $1$ and $p$
- The first few prime numbers are 2,3,5,7,...
- Is the set of prime numbers finite?
- Equivalently is there a largest prime?
- Euclid proved, around 300 BCE, that there cannot be a largest prime 
- Hence there must be infinitely many primes

## A fact about divisibility 

<center>

```
| = divisable, i.e. 2|4 reads 2 divides 4 / 4 is divisable by 2
 ```

| Observation |
| ------------- |
| If $n\|(a+b)\ and\ n\|a,\ then\ n\|b$ |

</center>

- Since $n|(a+b),a+b=u\cdot n$
- Since $n|a,a=v\cdot n$
- Therefore $a+b=vn+b=un$
- Hence $b=(u-v)n$

### Euclid's Prove of no largest prime and infinite primes

- Suppose the list of primes is finite, say 
  - $\{p_1,p_2,...,p_k\}$
- Consider $n=p_1\cdot p_2\cdot\cdot\cdot p_k+1$
- If n is a $composite\ number$, at least one prime $p_j$ is a factor, so $p_j|n$.
- Since $p_j$ appears in the product $p_1\cdot p_2\cdot\cdot\cdot p_j\cdot\cdot\cdot p_k$, we have $p_j|p_1\cdot p_2\cdot\cdot\cdot p_k$
- From our observation about divisibility, $p_j|n$ and $p_j|p_1\cdot p_2\cdot\cdot\cdot p_k$, we must also have $p_j|1$, which is not possible 
- So $n$ must also be prime, which is clearly bigger than $p_k$

## More about Primes

- Prime numbers have been extensively studied in mathematics
- Let $\pi(x)$ denote the numbers of primes smaller than $x$
- The $Prime\ Number\ Theorem$ says that $\pi(x)$ is approximately $\frac{x}{log(x)}$ for large values of x.
- Checking whether a number is a prime can be done efficiently -- <text style="color:#b6ff00">[Agrawal, Kayal, Saxena on 2002 at IIT Kanpur]
- No known efficient way to find factors of non-prime numbers 
- Large prime numbers are used in modern cryptography
- Essential for electronic commerce

# LEC 13 -  Why is a number irrational ?

## Irrational numbers

- The discovery of irrational numbers is attributed to the ancient Greeks
- Since Pythagoras, it was known that the diagonal of a unit square has length $\sqrt{2}$
- His followers spent many years trying to prove it was rational
- Hippasus is attributed with proving that $\sqrt{2}$ is irrational, around 500 BCE
- The follewers of Pythagoras were shocked by the discovery
- Allegedly, they drowened Hippasus at sea to supress this fact from the public

### Proof of Hippasus that $\sqrt{2}$ is not a rational number

- If $\sqrt{2}$ is rational, it can be written as a reduced fraction $\frac{p}{q}$, where $gcd(p,q)=1$
- From $\sqrt{2}=\frac{p}{q}$, squaring both sides, $2=\frac{p^2}{q^2}$
- Cross multiplying, $p^2=2q^2$ , $p^2$ is even
- The product of two odd numbers is odd and the product of two even numbers is even, since $p^2=p\cdot p$ , so $p$ is even, say $p=2a$
- So $p^2=(2a)^2=4a^2=2q^2$
- Therefore $q^2=2a^2$, $q^2$ is also even 
- by the same reasoning, $q$ is even , say $q=2b$
- S0 $p=2a$ and $q=2b$, which means $gcd(p,q)\geq2$, which contradicts our assumption that $\frac{p}{q}$ was in reduced form

## Summary 

- The proof of Hippasus follows a patern commomly used in mathematical reasoning
- To show that a fact $P$ holds, assume $not(P)$ and derive a contradiction
- Using similar strategy, we can show that for any natural number n that is not a perfect square, $\sqrt{n}$ is irrational

# LEC 14 - Set <text style="color:#cf0">v/s</text> Collection

## Set theory as a foundation for Mathematics

- A set is a collection of Items
- Use set theory to build up all of mathematics
  - Georg Cantor, Richard Dedekind 1970s 
- Natural numbers can be "defined" as follows 
  - 0 corresponds to empty set $\empty$
  - 1 is the set $\{0,\{0\}\} = \{\empty,\{\empty\}\}$
  - 2 is the set $\{1,\{\1}\}$
  - ...
  - $j+1$ is the set $\{j,\{j\}\}$
- Define arithmatic operations in terms of set building

## Russell's Paradox

- Set assumes the emptyset $\empty$ and basic set building operations
  - Union $\cup$, Intersection $\cap$, Cartesian product x,...
  - Set comprehension -- subset that satisfies a condition 
- Is every collection a set? Is there a set of all sets?
- Consider $S$, all sets that do not contain themselves
  - $S$ is a set, by set comprehension 
  - Does $S$ belong to $S$?
  - Yes? Any set that does not contain itself should be in $S$
  - NO? Any set that does not contain itself should not be in $S$
- <text style="color:#f55"> Russell's Paradox </text> --- also discovered by Ernst Zermelo
- Cannot have "set of all sets"

## Sets and collections

- Russell's Paradox tells us that not every collection can be called a set 
- Collection that is not a set is sometimes called a <text style="color:#f55">class</class>
- The paradox had a The paradox had a major on set theory as a logical foundation of Mathematics
- For us, just be sure that we always build new sets from existing sets
- Don't manufacture sets "out of thin air" --- "set" of all sets

# LEC 15 - Degrees of infinity 

## Are there degrees of infinity?

- Cardinality of a set is the number of elements 
- For finite sets, count the elements 
- What about infinite sets?
  - Is $\mathbb{N}$ smaller than $\mathbb{Z}$?
  - IS $\mathbb{Z}$ smaller than $\mathbb{Q}$?
  - Is $\mathbb{Q}$ smaller than $\mathbb{R}$?
- First systematically studied by Georg Cantor
- To compare cardinalities of infinite sets, use bijections 
  - One-to-one and onto function
  - Pairs elements form the sets so that none are left out

## Countable sets

- Staeting point of infinite sets is $\mathbb{N}$
- Suppose we have a bijection $f$ between $\mathbb{N}$
  - Enumerate $X$ as $\{f(0),f(1),...,\}$
  - $X$ can be "counted" via $f$
  - Such set is called <text style="color:#f55">countable

### is $\mathbb{Z}$ Countable?

- $\mathbb{Z}$ extends with negative integers 
- Intuitively, $\mathbb{Z}$ is twice as large as $\mathbb{N}$
- Can we setup a bijetion between $\mathbb{N}$ and $\mathbb{Z}?$
<center>

|...|$-4$|$-3$|$-2$|$-1$|$0$|$1$|$2$|$3$|$4$|...|
|--|--|--|--|--|--|--|--|--|--|--|
|...|$8$|$6$|$4$|$2$|$0$|$1$|$3$|$5$|$7$|...|

</center>

- The enumeration is effective
  - $f(0)=0$
  - For $i$ odd, $f(i)=\frac{(i+1)}{2}$
  - For $i$ even, $f(i)=-\frac{i}{2}$
- $\mathbb{Z}$ is countable

### is $\mathbb{Q}$ countable

- Q is dense, $\mathbb{Z}$ is descrete
- Are there more rationals than integers?
- There's an obvious bijection betweem $\mathbb{Z}\times\mathbb{Z}$ and $\mathbb{Q}$
  - $(p,q)\to \frac{p}{q}$
- Sufficient to check cardinality of $\mathbb{N}\times\mathbb{N}$
  - For simplicity, we restrict to $\mathbb{N}\times\mathbb{N}$
- Enumerate $\mathbb{N}\times\mathbb{N}$ diagonally
- Other enumeration strategies are also possible
- Can easily extend these to $\mathbb{Z}\times\mathbb{Z}$
- Hence $\mathbb{Q}$ is countable

<img src="https://notes.imt-decal.org/sets/n10-spiral.png" style="border-radius:10px">

### Is $\mathbb{R}$ countable?

- $\mathbb{R}$ extends $\mathbb{Q}$ by irrational numbers
- Cantor showed that $\mathbb{R}$ is not countable
- First a differnt set 
  - Infinite sequences over $\{0,1\}$
  - $010110...$
- Suppose there's dome enumeration 
- Flip $b_i$ in $s_i$
- Read off the <text style="color:#f40"> diagonal sequence 
- Diagonal swquences differ from each $s_i$ at $b_i$
- New sequence that is not part of the enumeration
<center>

|$s_1$|<text style="color:#b6FF00">0|0|0|0|0|0|0|0|0|...|
|----|----|----|----|----|----|----|----|----|----|----|
|$s_2$|1|<text style="color:#b6FF00">1|1|1|1|1|1|1|1|...|
|$s_3$|0|1|<text style="color:#b6FF00">0|1|0|1|0|1|0|...|
|$s_4$|1|0|1|<text style="color:#b6FF00">0|1|0|1|0|1|...|
|$s_5$|1|1|0|1|<text style="color:#b6FF00">0|1|1|0|1|...|
|$s_6$|0|0|1|1|0|<text style="color:#b6FF00">1|1|0|1|...|
|$s_7$|1|0|0|0|1|0|<text style="color:#b6FF00">0|0|1|...|
|$s_8$|0|0|1|1|0|0|1|<text style="color:#b6FF00">1|0|...|
|$s_9$|1|1|0|0|1|1|0|0|<text style="color:#b6FF00">1|...|
|$\vdots$|$\vdots$|$\vdots$|$\vdots$|$\vdots$|$\vdots$|$\vdots$|$\vdots$|$\vdots$|$\vdots$|<text style="color:#b6FF00">$\ddots$|

|$s_n$|<text style="color:#b6FF00">1|<text style="color:#b6FF00">0|<text style="color:#b6FF00">1|<text style="color:#b6FF00">1|<text style="color:#b6FF00">1|<text style="color:#b6FF00">0|<text style="color:#b6FF00">1|<text style="color:#b6FF00">0|<text style="color:#b6FF00">0|<text style="color:#b6FF00">$\dots$|
|----|----|----|----|----|----|----|----|----|----|----|
</center>
#### Infinite sequences over {0,1} can't be enumerated 

- Each sequence can be read as decimal fraction 
  - 0.010110110101....
- Injective function from {0,1} sequences to open interval $(0,1)\sube\mathbb{R}$
- Hence $(0,1)\sube\mathbb{R}$ can't be enumerated
- So $mathbb{R}$ is not countable

## Summery

- Any set that has a bijection from $\mathbb{N}$ is countable
- $\mathbb{Z}$ and $\mathbb{Q}$ are countable 
- $\mathbb{R}$ is not countable --- <tetx style="color:orange"> diagonalization
- Is there a set between $\mathbb{N}$ and $\mathbb{R}\ ?$
- <text style="color:#f05"> Continuum Hypothesis </text> --- one of the major questions in set theory
- Paul Cohen showed that you can neither prove neither disprove this Hypothesis within set theory
