# Goldbach-s-Conjecture
A Goldbach number is a positive even integer that can be expressed as the sum of two odd primes.[5] Since 4 is the only even number greater than 2 that requires the even prime 2 in order to be written as the sum of two primes, another form of the statement of Goldbach's conjecture is that all even integers greater than 4 are Goldbach numbers.

The expression of a given even number as a sum of two primes is called a Goldbach partition of that number. The following are examples of Goldbach partitions for some even numbers:

6 = 3 + 3
8 = 3 + 5
10 = 3 + 7 = 5 + 5
12 = 7 + 5
...
100 = 3 + 97 = 11 + 89 = 17 + 83 = 29 + 71 = 41 + 59 = 47 + 53

# heuristic Justification
Statistical considerations that focus on the probabilistic distribution of prime numbers present informal evidence in favour of the conjecture (in both the weak and strong forms) for sufficiently large integers: the greater the integer, the more ways there are available for that number to be represented as the sum of two or three other numbers, and the more "likely" it becomes that at least one of these representations consists entirely of primes.


Number of ways to write an even number n as the sum of two primes (4 ≤ n ≤ 1,000), (sequence A002375 in the OEIS)

Number of ways to write an even number n as the sum of two primes (4 ≤ n ≤ 1000000)
A very crude version of the heuristic probabilistic argument (for the strong form of the Goldbach conjecture) is as follows. The prime number theorem asserts that an integer m selected at random has roughly a {\displaystyle 1/\ln m}{\displaystyle 1/\ln m} chance of being prime. Thus if n is a large even integer and m is a number between 3 and n/2, then one might expect the probability of m and n − m simultaneously being prime to be {\displaystyle 1{\big /}{\big [}\ln m\,\ln(n-m){\big ]}}{\displaystyle 1{\big /}{\big [}\ln m\,\ln(n-m){\big ]}}. If one pursues this heuristic, one might expect the total number of ways to write a large even integer n as the sum of two odd primes to be roughly

{\displaystyle \sum _{m=3}^{n/2}{\frac {1}{\ln m}}{\frac {1}{\ln(n-m)}}\approx {\frac {n}{2(\ln n)^{2}}}.}{\displaystyle \sum _{m=3}^{n/2}{\frac {1}{\ln m}}{\frac {1}{\ln(n-m)}}\approx {\frac {n}{2(\ln n)^{2}}}.}
Since this quantity goes to infinity as n increases, we expect that every large even integer has not just one representation as the sum of two primes, but in fact has very many such representations.

This heuristic argument is actually somewhat inaccurate, because it assumes that the events of m and n − m being prime are statistically independent of each other. For instance, if m is odd, then n − m is also odd, and if m is even, then n − m is even, a non-trivial relation because, besides the number 2, only odd numbers can be prime. Similarly, if n is divisible by 3, and m was already a prime distinct from 3, then n − m would also be coprime to 3 and thus be slightly more likely to be prime than a general number. Pursuing this type of analysis more carefully, Hardy and Littlewood in 1923 conjectured (as part of their famous Hardy–Littlewood prime tuple conjecture) that for any fixed c ≥ 2, the number of representations of a large integer n as the sum of c primes {\displaystyle n=p_{1}+\cdots +p_{c}}{\displaystyle n=p_{1}+\cdots +p_{c}} with {\displaystyle p_{1}\leq \cdots \leq p_{c}}p_{1}\leq \cdots \leq p_{c} should be asymptotically equal to

{\displaystyle \left(\prod _{p}{\frac {p\gamma _{c,p}(n)}{(p-1)^{c}}}\right)\int _{2\leq x_{1}\leq \cdots \leq x_{c}:x_{1}+\cdots +x_{c}=n}{\frac {dx_{1}\cdots dx_{c-1}}{\ln x_{1}\cdots \ln x_{c}}},}{\displaystyle \left(\prod _{p}{\frac {p\gamma _{c,p}(n)}{(p-1)^{c}}}\right)\int _{2\leq x_{1}\leq \cdots \leq x_{c}:x_{1}+\cdots +x_{c}=n}{\frac {dx_{1}\cdots dx_{c-1}}{\ln x_{1}\cdots \ln x_{c}}},}
where the product is over all primes p, and {\displaystyle \gamma _{c,p}(n)}\gamma _{c,p}(n) is the number of solutions to the equation {\displaystyle n=q_{1}+\cdots +q_{c}\mod p}n=q_{1}+\cdots +q_{c}\mod p in modular arithmetic, subject to the constraints {\displaystyle q_{1},\ldots ,q_{c}\neq 0\mod p}{\displaystyle q_{1},\ldots ,q_{c}\neq 0\mod p}. This formula has been rigorously proven to be asymptotically valid for c ≥ 3 from the work of Vinogradov, but is still only a conjecture when {\displaystyle c=2}c=2.[citation needed] In the latter case, the above formula simplifies to 0 when n is odd, and to

{\displaystyle 2\Pi _{2}\left(\prod _{p\mid n;p\geq 3}{\frac {p-1}{p-2}}\right)\int _{2}^{n}{\frac {dx}{(\ln x)^{2}}}\approx 2\Pi _{2}\left(\prod _{p\mid n;p\geq 3}{\frac {p-1}{p-2}}\right){\frac {n}{(\ln n)^{2}}}}{\displaystyle 2\Pi _{2}\left(\prod _{p\mid n;p\geq 3}{\frac {p-1}{p-2}}\right)\int _{2}^{n}{\frac {dx}{(\ln x)^{2}}}\approx 2\Pi _{2}\left(\prod _{p\mid n;p\geq 3}{\frac {p-1}{p-2}}\right){\frac {n}{(\ln n)^{2}}}}
when n is even, where {\displaystyle \Pi _{2}}\Pi _{2} is Hardy–Littlewood's twin prime constant

{\displaystyle \Pi _{2}:=\prod _{p\geq 3}\left(1-{\frac {1}{(p-1)^{2}}}\right)=0.6601618158\ldots .}{\displaystyle \Pi _{2}:=\prod _{p\geq 3}\left(1-{\frac {1}{(p-1)^{2}}}\right)=0.6601618158\ldots .}
This is sometimes known as the extended Goldbach conjecture. The strong Goldbach conjecture is in fact very similar to the twin prime conjecture, and the two conjectures are believed to be of roughly comparable difficulty.

The Goldbach partition functions shown here can be displayed as histograms, which informatively illustrate the above equations.
