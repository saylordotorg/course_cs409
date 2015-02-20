---
layout: default
title: "CS409: Cryptography"
course_description: "A study of the conventional encryption systems and classical cryptography, exploring the use of secret key (or symmetric) cryptography, public-key (or asymmetric) cryptography, and hash functions."
next: ../Unit02
previous: ../Intro
---
**Unit 1: Introduction into Cryptography** <span id="1"></span> 
*This unit provides an overview of cryptography, the study of
information-hiding and verification.  Cryptography insures the
confidentiality/privacy, message integrity, authentication, and
non-repudiation of information.  There are two basic types of ciphers
used: the symmetric key cipher, which uses the same key for the same
message, and the asymmetric key cipher, which uses different keys for
encoding and decoding the same message. *  
  
 *This unit will also go over the basics of information theory so that
students can get a feel for message encoding before addressing various
classical ciphers, which can now be easily cryptanalyzed and broken. 
Lastly, we will take a look at the methods and techniques used to
cryptanalyze any algorithm that enciphers text.*

**Unit 1 Time Advisory**  
This unit will take approximately 16 hours to complete.

☐    Subunit 1.1: 1 hour

☐    Subunit 1.2: 1 hour

☐    Subunit 1.3: 2 hours

☐    Subunit 1.4: 2 hours

☐    Subunit 1.5: 1 hour

☐    Subunit 1.6: 9 hours

**Unit1 Learning Outcomes**  
Upon successful completion of this unit, students will be able to:

-   Explain the difference between symmetric and asymmetric key ciphers.
-   Define cryptography’s goals.
-   Use the formula for determining the number of bits required in an
    optimal code.
-   Define most common methods of cryptanalysis for classical ciphers.

**1.1 Introduction** <span id="1.1"></span> 
-   **Reading: Wikibooks’ “Cryptography: Introduction”**
    Link: Wikibooks’ [“Cryptography:
    Introduction](http://www.saylor.org/site/wp-content/uploads/2012/07/Introduction.pdf)[”](http://www.saylor.org/site/wp-content/uploads/2012/07/Introduction.pdf)
    (PDF)  
        
     Instructions: Read the article for a general introduction to
    cryptography.  Learn the terms in bold font and familiarize yourself
    with the common goals and forms of cryptography.  This reading
    covers subunits 1.1.1 through 1.1.3.    
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/).  You can find
    the original Wikibooks version of this article
    [here](http://en.wikibooks.org/wiki/Cryptography/Introduction).

**1.1.1 Basic Vocabulary** <span id="1.1.1"></span> 
**1.1.2 Common Goals in Cryptography** <span id="1.1.2"></span> 
**1.1.3 Common Forms of Cryptography** <span id="1.1.3"></span> 
**1.2 History of Cryptography** <span id="1.2"></span> 
-   **Reading: Wikibooks’ “Cryptography: History”**
    Link: Wikibooks’ [“Cryptography:
    History”](http://www.saylor.org/site/wp-content/uploads/2012/07/History.pdf)
    (PDF)  
        
     Instructions: Read this article to familiarize yourself with
    cryptography’s history.  
        
     Terms of Use: The article above is released under a [Creative
    Commons Attribution-Share-Alike License
    3.0](http://creativecommons.org/licenses/by-sa/3.0/).  You can find
    the original Wikibooks version of this article
    [here](http://en.wikibooks.org/wiki/Cryptography/History).

**1.3 Basics of Information Theory** <span id="1.3"></span> 
-   **Reading: Computer Science at Carnegie Mellon: David Touretzky’s
    “Basics of Information Theory”**
    Link: Computer Science at Carnegie Mellon: David
    Touretzky’s [“Basics of Information
    Theory”](http://www.cs.cmu.edu/~dst/Tutorials/Info-Theory/) (HTML)  
        
     Instructions: Read this webpage to learn about information theory
    and get a feel for how messeges can be encoded.  Make sure you do
    the exercise listed on the page under “Variable Length Codes”
    section.  This reading covers subunits 1.3.1-1.3.4.    
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**1.3.1 Efficient Encodings** <span id="1.3.1"></span> 
**1.3.2 Variable Length Codes** <span id="1.3.2"></span> 
**1.3.3 Measuring Information Content** <span id="1.3.3"></span> 
**1.3.4 The Intuition Behind the -P log P Formula** <span
id="1.3.4"></span> 
**1.4 Basic Cryptanalysis** <span id="1.4"></span> 
-   **Reading: Practical Cryptography’s “Cryptanalysis”**
    Link: Practical Cryptography’s
    [“Cryptanalysis](http://practicalcryptography.com/cryptanalysis/)[”](http://practicalcryptography.com/cryptanalysis/)
    (HTML)  
      
     Instructions: Read the webpage to learn about the basic
    cryptanalysis techniques.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**1.4.1 Monogram, Bigram, and Trigram Frequency Counts** <span
id="1.4.1"></span> 
-   **Reading: Practical Cryptography’s “Monogram, Bigram, and Trigram
    Frequency Counts”**
    Link: Practical Cryptography’s [“Monogram, Bigram, and Trigram
    Frequency
    Counts”](http://practicalcryptography.com/cryptanalysis/text-characterisation/monogram-bigram-and-trigram-frequency-counts/) (HTML)  
      
     Instructions: Read the webpage to learn about various cryptanalysis
    techniques.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**1.5 Alice and Bob Go to Washington: A Cryptographic Theory of Politics
and Policy** <span id="1.5"></span> 
-   **Lecture: CRYPTO: Edward Felten's “Alice and Bob Go to Washington:
    A Cryptographic Theory of Politics and Policy”**
    Link: CRYPTO: Edward Felten's [“Alice and Bob Go to Washington: A
    Cryptographic Theory of Politics and
    Policy”](http://www.iacr.org/conferences/crypto2009/videos/08_Edward_Felten_-_Alice_and_Bob_go_to_Washington.html) (Flash)  
        
     Also available in:  
     [Mp4
    Video](http://www.iacr.org/conferences/crypto2009/videos/08_Edward_Felten_-_Alice_and_Bob_go_to_Washington.mp4)  
        
     Instructions: Watch this 1-hour video about cryptography and
    politics.  It discusses the choices national leaders are making
    about technology.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**1.6 Stats in Code** <span id="1.6"></span> 
-   **Activity: home.cogeco.ca: John Russell’s “Frequency Counting”**
    Link: home.cogeco.ca: John Russell’s [“Frequency
    Counting](http://www.saylor.org/site/wp-content/uploads/2012/07/Cryptology-Programs.pdf)[”](http://www.saylor.org/site/wp-content/uploads/2012/07/Cryptology-Programs.pdf)
    (PDF)  
        
     Instructions: If you do not have java compiler on your computer,
    install Java on your computer via
    [www.java.com](http://www.java.com/).   Then, create a java language
    program that performes a frequency counting.  You can see how to
    compile a java code via the java tutorials provided at
    [download.oracle.com](http://download.oracle.com/javase/tutorial/getStarted/cupojava/win32.html).
     One possible solution can be found via the link above, under the
    Frequency Counting section.  Study the solution code only after you
    have solved the problem or spent a substantial amount of time
    working on it (it could take you up to 9 hours).    
        
     Terms of Use: The linked material above has been reposted by the
    kind permission of John Russell, and can be viewed in its original
    from [here](http://home.cogeco.ca/~cipher/cyprogs.htm).  Please note
    that this material is under copyright and cannot be reproduced in
    any capacity without explicit permission from the copyright holder. 


