---
layout: default
title: "CS409: Cryptography"
course_description: "A study of the conventional encryption systems and classical cryptography, exploring the use of secret key (or symmetric) cryptography, public-key (or asymmetric) cryptography, and hash functions."
next: ../Unit06
previous: ../Unit04
---
**Unit 5: The RSA Cryptosystem and Factoring Integers** <span
id="5"></span> 
*In this unit, we will learn the basic idea behind public key
cryptography and explain in detail RSA as the most important example of
public key cryptography.  Next, we will discuss the algorithms used to
determine whether an input number is prime.  As noted earlier, these
algorithms are important in public key cryptography because encryption
depends on the factorization of prime numbers.  This unit will present
the mathematical background you need in order to understand these
algorithms and in turn get a better picture of public key
cryptography. *

**Unit 5 Time Advisory**  
This unit will take approximately 23 hours to complete.

☐    Subunit 5.1: 2 hours

☐    Subunit 5.2: 5 hours

☐    Subunit 5.3: 7 hours

☐    Subunit 5.4: 9 hours

**Unit5 Learning Outcomes**  
Upon successful completion of this unit, students will be able to:

-   Describe the idea behind public key cryptography.
-   Apply the RSA cryptography system to a practical problem.
-   Test whether a large integer is prime via the naive method and
    probabilistic testing.
-   Describe Euclid’s algorithm and prove the Chinese Reminder Theorem.
-   Describe the Legendre and Jacobi symbols.
-   Define a subgroup.
-   Explain the Pollard p-1 algorithm and Pollard Rho algorithm.
-   Explain the Shanks’ Square Forms Factorization algorithm.
-   Explain the Solovay-Strassen test.
-   Define strong pseudoprime.
-   Expline the Miller-Rabin Prime test.

**5.1 Introduction** <span id="5.1"></span> 
-   **Reading: PlanetMath: Andrew Ross’s “Public Key Cryptography”**
    Link: PlanetMath: Andrew Ross’s [“Public Key
    Cryptography](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.11.pdf)[”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.11.pdf)
    (PDF)  
        
     Instructions: Read the linked webpage for introduction to public
    key cryptography.  
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of Andrew Ross, and can be viewed in its original
    from
    [here](http://planetmath.org/encyclopedia/PublicKeyCryptography.html).  Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder.<span class="Apple-style-span"
    style="border-collapse: collapse; font-family: arial, sans-serif; font-size: 13px; color: rgb(0, 0, 0); "><span> </span></span>

**5.1.1 Example of Public Key Cryptography** <span id="5.1.1"></span> 
-   **Reading: PlanetMath: Andrew Ross’s “RSA”**
    Link: PlanetMath: Andrew Ross’s
    [“RSA](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.1.12.pdf)[”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.1.12.pdf)
    (PDF)  
        
     Instructions: Read the linked webpage above to learn whatRSA is. 
    Take for granted the Chinese Reminder theorem, which is explained in
    a later subunit.  
      
     Terms of Use: The linked material above has been reposted by the
    kind permission of Andrew Ross, and can be viewed in its original
    from
    [here](http://planetmath.org/encyclopedia/RSACryptosystem.html).  Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder. 

**5.1.2 Primality Testing** <span id="5.1.2"></span> 
-   **Reading: Wikipedia’s “Primality Test”**
    Link: Wikipedia’s [“Primality
    Test](https://resources.saylor.org/archived/wp-content/uploads/2012/07/Primality-test1.pdf)[”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/Primality-test1.pdf)
    (PDF)  
        
     Instructions: Read this article on primality testing, which is
    crucial to the security of public-key cryptography.  Make sure you
    understand the naive tests, probabilistic tests, and fast
    deterministic tests.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/).  You can find
    the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/Primality_test).

**5.2 Math Background** <span id="5.2"></span> 
**5.2.1 Euclid's Algorithm** <span id="5.2.1"></span> 
-   **Reading: PlanetMath: Robert Milson’s “Euclid's Algorithm”**
    Link: PlanetMath: Robert Milson’s [“Euclid's
    Algorithm](http://%20www.saylor.org/site/wp-content/uploads/2012/07/CS409-5.2.11.pdf)[”](http://%20www.saylor.org/site/wp-content/uploads/2012/07/CS409-5.2.11.pdf)
    (PDF)             
        
     Instructions: Read the linked webpage above to learn how Euclid's
    algorithm works.  Work through the given example.  
      
     Terms of Use: The linked material above has been reposted by the
    kind permission of Robert Milson, and can be viewed in its original
    from
    [here](http://planetmath.org/encyclopedia/EuclideanAlgorithm.html).  Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder.

**5.2.2 Chinese Remainder Theorem** <span id="5.2.2"></span> 
-   **Reading: PlanetMath: Chi Woo’s “Chinese Remainder Theorem”**
    Link: PlanetMath: Chi Woo’s [“Chinese Remainder
    Theorem](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.2.21.pdf)[”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.2.21.pdf)
    (PDF)  
        
     Instructions: Read the linked webpage to learn how Chinese
    Remainder theorem works.  
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of Chi Woo, and can be viewed in its original from
    [here](http://planetmath.org/encyclopedia/ChineseRemainderTheorem.html).  Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder.<span class="Apple-style-span"
    style="border-collapse: collapse; font-family: arial, sans-serif; font-size: 13px; color: rgb(0, 0, 0); "><span> </span></span>

**5.2.3 Legendre Symbol** <span id="5.2.3"></span> 
-   **Reading: PlanetMath: Alvaro Lozano Robledo’s “Legendre Symbol”**
    Link: PlanetMath: Alvaro Lozano Robledo’s [“Legendre
    Symbol](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.2.31.pdf)[”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.2.31.pdf)
    (PDF)  
        
     Instructions: This reading will define the Legendre symbol.  
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of  Alvaro Lozano Robledo, and can be viewed in its
    original from
    [here](http://planetmath.org/encyclopedia/LegendreSymbol.html).  Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder. 

**5.2.4 Calculating the Jacobi Symbol** <span id="5.2.4"></span> 
-   **Reading: PlanetMath: Christoph Bergemann’s “Jacobi Symbol” and
    “Calculating the Jacobi Symbol”**
    Link: PlanetMath: Christoph Bergemann’s [“Jacobi
    Symbol”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.2.41.pdf) (PDF)
    and [“Calculating the Jacobi
    Symbol](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.2.4-21.pdf)[”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.2.4-21.pdf)
    (PDF)  
        
     Instructions: Read these webpages.  
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of  Christoph Bergemann, and can be viewed in its
    original from
    [here](http://planetmath.org/encyclopedia/JacobiSymbol.html) and
    [here](http://planetmath.org/encyclopedia/CalculatingTheJacobiSymbol.html).  Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder. 

**5.2.5 Subgroup** <span id="5.2.5"></span> 
-   **Reading: PlanetMath: Yann Lamontagne’s “Subgroup”**
    Link: PlanetMath: Yann Lamontagne’s
    [“Subgroup](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.2.51.pdf)[”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.2.51.pdf)
    (PDF)  
        
     Instructions: Read the linked webpage above to learn the definition
    of a subgroup.  
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of  Yann Lamontagne, and can be viewed in its
    original from
    [here](http://planetmath.org/encyclopedia/TrivialSubgroup.html).  Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder. 

**5.3 Prime Factorization Algorithms (More Math)** <span
id="5.3"></span> 
-   **Reading: Wolfram Mathworld: Eric Weisstein's “Prime Factorization
    Algorithms”**
    Link: Wolfram Mathworld: Eric Weisstein’s [“Prime Factorization
    Algorithms](http://mathworld.wolfram.com/PrimeFactorizationAlgorithms.html)[”](http://mathworld.wolfram.com/PrimeFactorizationAlgorithms.html)
    (HTML)  
        
     Instructions: Read the linked webpage for an introduction to prime
    factorization.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**5.3.1 Integer Factorization** <span id="5.3.1"></span> 
-   **Reading: PlanetMath: John Smith’s “Integer Factorization”**
    Link: PlanetMath: John Smith’s [“Integer
    Factorization](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.3.1.pdf)[”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.3.1.pdf)
    (PDF)  
        
     Instructions: Read the linked webpage to learn about integer
    factorization.  
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of John Smith, and can be viewed in its original
    from
    [here](http://planetmath.org/encyclopedia/PrimeFactorization.html).  Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder. 

**5.3.2 The Pollard p-1 Algorithm** <span id="5.3.2"></span> 
-   **Reading: PlanetMath: John Smith’s “Pollard p-1 Algorithm”**
    Link: PlanetMath: John Smith’s [“Pollard p-1
    Algorithm](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.3.21.pdf)[”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.3.21.pdf)
    (PDF)  
        
     Instructions: Read the linked webpage to learn how to factor an
    integer with Pollard's p-1 algorithm.  
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of John Smith, and can be viewed in its original
    from
    [here](http://planetmath.org/encyclopedia/PollardsP1Algorithm.html).  Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder. 

**5.3.3 The Pollard Rho Algorithm** <span id="5.3.3"></span> 
-   **Reading: PlanetMath: John Smith’s “Pollard Rho Algorithm”**
    Link: PlanetMath: John Smith’s [“Pollard Rho
    Algorithm](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.3.3.pdf)[”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.3.3.pdf)
    (PDF)  
        
     Instructions: Read the linked webpage to learn how to factor an
    integer with Pollard's Rho algorithm.  
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of John Smith, and can be viewed in its original
    from
    [here](http://planetmath.org/encyclopedia/PollardsRhoAlgorithm.html).  Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder.<span class="Apple-style-span"
    style="border-collapse: collapse; font-family: arial, sans-serif; font-size: 13px; color: rgb(0, 0, 0); "><span> </span></span>

**5.3.4 Shanks' Square Forms Factorization** <span id="5.3.4"></span> 
-   **Reading: Wikipedia’s “Shanks' Square Forms Factorization”**
    Link: Wikipedia’s [“Shanks' Square Forms
    Factorization”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/Shanks-square-forms-factorization.pdf)
    (PDF)  
        
     Instructions: Read the linked article to learn about Shanks' square
    forms factorization.  Make sure you understand the algorithm and the
    examples given.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/).  You can find
    the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/Shanks'_square_forms_factorization).

**5.3.5 The Solovay-Strassen Algorithm** <span id="5.3.5"></span> 
-   **Reading: PlanetMath: Christoph Bergemann’s “Solovay-Strassen
    Test”**
    Link: PlanetMath: Christoph Bergemann’s [“Solovay-Strassen
    Test](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.3.5.pdf)[”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.3.5.pdf)
    (PDF)  
        
     Instructions: Read the linked webpage to learn the how
    Solovay-Strassen test works.  If some definitions are not clear,
    click on the links provided on the website.  
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of Christoph Bergemann, and can be viewed in its
    original form
    [here](http://planetmath.org/encyclopedia/SolovayStrassenTest.html).  Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder. 

**5.3.6 Strong Pseudoprimes** <span id="5.3.6"></span> 
-   **Reading: Wikipedia’s “Strong Pseudoprime”**
    Link: Wikipedia’s [“Strong
    Pseudoprime](https://resources.saylor.org/archived/wp-content/uploads/2012/07/Strong-pseudoprime.pdf)[”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/Strong-pseudoprime.pdf)
    (PDF)  
        
     Instructions: Read the linked article to learn the definitions and
    properties of pseudoprime numbers.  Go through the examples.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/).  You can find
    the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/Strong_pseudoprime).

**5.3.7 Miller-Rabin Prime Test** <span id="5.3.7"></span> 
-   **Reading: PlanetMath: Christoph Bergemann’s “Miller-Rabin Prime
    Test”**
    Link: PlanetMath: Christoph Bergemann’s [“Miller-Rabin Prime
    Test](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.3.7.pdf)[”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.3.7.pdf)
    (PDF)  
        
     Instructions: Read the linked webpage to learn the how Miller-Rabin
    Primetest works.  
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of Christoph Bergemann, and can be viewed in its
    original from
    [here](http://planetmath.org/?op=getobj&from=objects&name=MillerRabinPrimeTest).  Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder. 

**5.4 Miller-Rabin Primality Test in Code** <span id="5.4"></span> 
-   **Activity: LiteratePrograms’s “Miller-Rabin Primality Test”**
    Link: LiteratePrograms’s [“Miller-Rabin Primality
    Test](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.4.pdf)[”](https://resources.saylor.org/archived/wp-content/uploads/2012/07/CS409-5.4.pdf)
    (PDF)  
        
     Instructions: Create a java language program that performs
    Miller-Rabin primality test.  One possible solution can be found via
    the link above.  Study the solution code only after you have solved
    the problem or spent a substantial amount of time working on it (it
    could take you up to 9 hours).    
        
     Terms of Use: This material is part of the public domain. 


