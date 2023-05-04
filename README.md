Download Link: https://assignmentchef.com/product/solved-cs70-homework4
<br>
Before you start your homework, state briefly how you worked on it. Who else did you work with? List names and email addresses. (In case of homework party, you can just describe the group.)

Find all solutions (modulo the corresponding modulus) to the following equations. Prove that there are no other solutions (in a modular setting) to each equation.

<ul>

 <li>2<em>x </em>≡ 5 (mod 15)</li>

 <li>2<em>x </em>≡ 5 (mod 16) (c) 5<em>x </em>≡ 10 (mod 25)</li>

</ul>

<h1>2          Euclid’s Algorithm</h1>

<ul>

 <li>Use Euclid’s algorithm from lecture to compute the greatest common divisor of 527 and 323. List the values of <em>x </em>and <em>y </em>of all recursive calls.</li>

 <li>Use extended Euclid’s algorithm from lecture to compute the multiplicative inverse of 5 mod</li>

</ul>

<ol start="27">

 <li>List the values of <em>x </em>and <em>y </em>and the returned values of all recursive calls.</li>

</ol>

<ul>

 <li>Find <em>x </em>(mod 27) if 5<em>x</em>+26 ≡ 3 (mod 27). You can use the result computed in (b).</li>

 <li>Assume <em>a</em>, <em>b</em>, and <em>c </em>are integers and <em>c </em><em>&gt; </em> Prove or disprove: If <em>a </em>has no multiplicative inverse mod <em>c</em>, then <em>ax </em>≡ <em>b </em>(mod <em>c</em>) has no solution.</li>

</ul>

<h1>3          Modular Exponentiation</h1>

Compute the following:

<ul>

 <li>13<sup>2018 </sup>(mod 12)</li>

 <li>8<sup>11111 </sup>(mod 9)</li>

 <li>7<sup>256 </sup>(mod 11)</li>

 <li>3<sup>160 </sup>(mod 23)</li>

</ul>

<h1>4          Euler’s Totient Function</h1>

Euler’s totient function is defined as follows:

<em>φ</em>(<em>n</em>)= |{<em>i </em>: 1 ≤ <em>i </em>≤ <em>n</em><em>,</em>gcd(<em>n</em><em>,i</em>)= 1}|

In other words, <em>φ</em>(<em>n</em>) is the total number of positive integers less than or equal to <em>n </em>which are relatively prime to it. Here is a property of Euler’s totient function that you can use without proof:

For <em>m</em><em>,n </em>such that gcd(<em>m</em><em>,n</em>) = 1, <em>φ</em>(<em>mn</em>)=<em>φ</em>(<em>m</em>)·<em>φ</em>(<em>n</em>).

<ul>

 <li>Let <em>p </em>be a prime number. What is <em>φ</em>(<em>p</em>)?</li>

 <li>Let <em>p </em>be a prime number and <em>k </em>be some positive integer. What is <em>φ</em>(<em>p<sup>k</sup></em>)?</li>

 <li>Let <em>p </em>be a prime number and <em>a </em>be a positive integer smaller than <em>p</em>. What is <em>a<sup>φ</sup></em><sup>(<em>p</em></sup><sup>) </sup>(mod <em>p</em>)? <em>(Hint: use Fermat’s Little Theorem.)</em></li>

 <li>Let <em>b </em>be a positive integer whose prime factors are <em>p</em><sub>1</sub><em>, p</em><sub>2</sub><em>,…, p<sub>k</sub></em>. We can write <em>b </em><em>p</em><em> … p<sup>α</sup><sub>k</sub></em><em><sup>k</sup></em>.</li>

</ul>

Show that for any <em>a </em>relatively prime to <em>b</em>, the following holds:

∀<em>i </em>∈ {1<em>,</em>2<em>,…,k</em>}<em>, </em><em>a<sup>φ</sup></em><sup>(<em>b</em></sup><sup>) </sup>≡ 1 (mod <em>p<sub>i</sub></em>)

<h1>5          FLT Converse</h1>

Recall that the FLT states that, given a prime <em>n</em>, <em>a<sup>n</sup></em><sup>−1 </sup>≡ 1 (mod <em>n</em>) <em>for all </em>1 ≤ <em>a </em>≤ <em>n</em>−1. Note that it says nothing about when <em>n </em>is composite.

Can the FLT condition (<em>a<sup>n</sup></em><sup>−1 </sup>≡ 1 mod <em>n</em>) hold for some or even all <em>a </em>if <em>n </em>is composite? This problem will investigate both possibilities. It turns out that unlike in the prime case, we need to restrict ourselves to looking at <em>a </em>that are relatively prime to <em>n</em>. (Note that if <em>n </em>is prime, then every <em>a </em><em>&lt; n </em>is relatively prime to <em>n</em>). Because of this restriction, let’s define

<em>S</em>(<em>n</em>)= {<em>i </em>: 1 ≤ <em>i </em>≤ <em>n</em><em>,</em>gcd(<em>n</em><em>,i</em>)= 1}<em>,</em>

so | <em>S </em>| is the total number of possible choices for <em>a</em>.

<ul>

 <li>Prove that for every <em>a </em>and <em>n </em>that are not relatively prime, FLT condition fails. In other words, for every <em>a </em>and <em>n </em>such that gcd(<em>n</em><em>,a</em>) 6= 1, we have <em>a<sup>n</sup></em><sup>−1 </sup>≡6 1 (mod <em>n</em>).</li>

 <li>Prove that the FLT condition fails for most choices of <em>a </em>and <em>n</em>. More precisely, show that if we can find a single <em>a </em>∈ <em>S</em>(<em>n</em>) such that <em>a<sup>n</sup></em><sup>−1 </sup>≡6 1 (mod <em>n</em>), we can find at least |<em>S</em>(<em>n</em>)|<em>/</em>2 such <em>a</em>. (Hint: You’re almost there if you can show that the set of numbers that fail the FLT condition is at least as large as the set of numbers that pass it. A clever bijection may be useful to compare set sizes.)</li>

</ul>

The above tells us that if a composite number fails the FLT condition for even one number relatively prime to it, then it fails the condition for most numbers relatively prime to it. However, it doesn’t rule out the possibility that some composite number <em>n </em>satisifes the FLT condition entirely: <em>for all a </em>relatively prime to <em>n</em>, <em>a<sup>n</sup></em><sup>−1 </sup>≡ 1 mod <em>n</em>. It turns out such numbers do exist, but they were found through trial-and-error! We will prove one of the conditions on <em>n </em>that make it easy to verify the existence of these numbers.

<ul>

 <li>First, show that if <em>a </em>≡ <em>b </em>mod <em>m</em><sub>1 </sub>and <em>a </em>≡ <em>b </em>mod <em>m</em><sub>2</sub>, with gcd(<em>m</em><sub>1</sub><em>,m</em><sub>2</sub>) = 1, then <em>a </em>≡ <em>b </em>(mod <em>m</em><sub>1</sub><em>m</em><sub>2</sub>).</li>

 <li>Let <em>n </em>= <em>p</em><sub>1</sub><em>p</em><sub>2 </sub>·· <em>p<sub>k </sub></em>where <em>p<sub>i </sub></em>are distinct primes and <em>p<sub>i </sub></em>−1 | <em>n</em>−1 for all <em>i</em>. Show that <em>a<sup>n</sup></em><sup>−1 </sup>≡ 1 (mod <em>n</em>) for all <em>a </em>∈ <em>S</em>(<em>n</em>)</li>

 <li>Verify that for all <em>a </em>coprime with 561, <em>a</em><sup>560 </sup>≡ 1 (mod 561).</li>

</ul>