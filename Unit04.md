---
layout: default
title: "CS409: Cryptography"
course_description: "A study of the conventional encryption systems and classical cryptography, exploring the use of secret key (or symmetric) cryptography, public-key (or asymmetric) cryptography, and hash functions."
next: ../Unit05
previous: ../Unit03
---
**Unit 4: Hash Functions** <span id="4"></span> 
*This unit will introduce the concept of “hash” and then present the
important MD5 and SHA-1 hash functions.  (MD5 is a widely used
cryptographic hash function with a 128-bit hash value, and SHA-1 is a
cryptographic hash function designed by the National Security Agency.) 
We will finish the unit with a look at message authentication code,
sometimes called a “keyed hash function.”*

**Unit 4 Time Advisory**  
This unit will take approximately 19 hours to complete.

☐    Subunit 4.1: 3 hours

☐    Subunit 4.2: 7 hours

☐    Subunit 4.2.1: 3 hours  
  
 ☐    Subunit 4.2.2: 3 hours  
  
 ☐    Subunit 4.2.3: 1 hour

☐    Subunit 4.3: 9 hours

**Unit4 Learning Outcomes**  
Upon successful completion of this unit, students will be able to:

-   Explain what cryptographic hash is.
-   Use hash function in a computer.
-   Describe MD5 hash function and the collision vulnerabilities
    associated with it.
-   Describe SHA-1 hash function.

**4.1 Cryptographic Hash** <span id="4.1"></span> 
-   **Reading: Unixwiz’s “An Illustrated Guide to Cryptographic
    Hashes”**
    Link: Unixwiz’s [“An Illustrated Guide to Cryptographic
    Hashes](http://unixwiz.net/techtips/iguide-crypto-hashes.html)[”](http://unixwiz.net/techtips/iguide-crypto-hashes.html)
    (HTML)  
        
     Instructions: Read the web page about cryptographic hashs. 
    Understand what hash is, how hash works, how to use it with UNIX,
    and issues related to collisions.  This reading covers subunits
    4.1.1 through 4.1.8.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**4.1.1 What Is a Cryptographic Hash?** <span id="4.1.1"></span> 
**4.1.2 Hashes Are Digests, Not Encryption** <span id="4.1.2"></span> 
**4.1.3 How Are Hashes Used?** <span id="4.1.3"></span> 
**4.1.4 But What About Collisions?** <span id="4.1.4"></span> 
**4.1.5 What's inside a Cryptographic Hash?** <span id="4.1.5"></span> 
**4.1.6 Collision Resistance in More Detail** <span id="4.1.6"></span> 
**4.1.7 So What's the Big News?** <span id="4.1.7"></span> 
**4.1.8 What Does This Mean?** <span id="4.1.8"></span> 
**4.2 Cryptographic Hash Functions** <span id="4.2"></span> 
**4.2.1 MD5** <span id="4.2.1"></span> 
-   **Reading: Wikipedia’s “MD5”**
    Link: Wikipedia’s
    [“MD5](http://www.saylor.org/site/wp-content/uploads/2012/07/MD51.pdf)[”](http://www.saylor.org/site/wp-content/uploads/2012/07/MD51.pdf)
    (PDF)  
        
     Instructions: Read about the MD5, which is a widely used
    cryptographic hash function.  Make sure you understand the MD5
    algorithm.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/).  You can find
    the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/MD5).

**4.2.2 SHA-1** <span id="4.2.2"></span> 
-   **Reading: Wikipedia’s “SHA-1”**
    Link: Wikipedia’s
    [“SHA-1](http://www.saylor.org/site/wp-content/uploads/2012/07/SHA-1-1.pdf)[”](http://www.saylor.org/site/wp-content/uploads/2012/07/SHA-1-1.pdf)
    (PDF)  
        
     Instructions: Read about the cryptographic hash function designed
    by the National Security Agency.  Make sure you understand SHA-1
    pseudo code.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/).  You can find
    the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/SHA-1).

**4.2.3 Message Authentication Code** <span id="4.2.3"></span> 
-   **Reading: Wikipedia’s “Message Authentication Code”**
    Link: Wikipedia’s [“Message Authentication
    Code](http://www.saylor.org/site/wp-content/uploads/2012/07/Message-authentication-code1.pdf)[”](http://www.saylor.org/site/wp-content/uploads/2012/07/Message-authentication-code1.pdf)
    (PDF)  
        
     Instructions: Read the linked article about message authentication
    code.  Make sure you understand the example given on the web site.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/).  You can find
    the original Wikipedia version of this article
    [here](http://en.wikipedia.org/wiki/Message_authentication_code).

**4.3 Cryptographic Hashing Function in Code** <span id="4.3"></span> 
-   **Reading: OWASP’s “Cryptographic Hashing Function”**
    Link: OWASP’s [“Cryptographic Hashing
    Function](http://www.saylor.org/site/wp-content/uploads/2012/07/CS409-4.3.pdf)[”](http://www.saylor.org/site/wp-content/uploads/2012/07/CS409-4.3.pdf)
    (PDF)  
        
     Instructions: Create a Java language program that runs
    cryptographic hashing function.  One possible solution can be found
    via the link above.  Study the solution code only after you have
    solved the problem or spent a substantial amount of time working on
    it (it could take you up to 9 hours).    
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of OWASP, and can be viewed in its original
    from [here](https://www.owasp.org/index.php/Hashing_Java#Definition_of__cryptographic_Hashing_function:). Please
    note that this material is under copyright and cannot be reproduced
    in any capacity without explicit permission from the copyright
    holder.  <span style="display: none; "> </span>


