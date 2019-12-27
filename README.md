# RSA
RSA in code 

#### what
RSA is one of the first cryptosystem for public-key encrytion, named by Ron Rives, Adi Shamir, and Leonard Adleman.
The encrytion key is different from the decription key that is kept scret (private).

#### why
It's wilded sued for trasmitting data scurely.

#### How
The **asymmetry** is rely on the pracitical difficulty of fatorization of the product of two large prime numbers called "factoring problems".


#### Operation
1. Pick two prime numbers p and q (p!=q)
2. n=pq which is modulus of both keys.
3. Calculate P=(p-1)(q-1) (where P is toitient, the # of positive integers not more than a specified int that are relatively prime to it.)
4. Find e which is the public key
where e > 1 and coprime to P, i.e. gcd (P, e) == 1, 
and e < P
5. Choose d which is the private key
and satisfies the equation d * e % p == 1
6. Abandon p and q
then,
public key  : N,e
private key : N,d
7. Cipher text is encrypted by the equation c= m^e % n
where m is the message
8.With c and d the massage is decrypted euqation m = c ^ d % n


