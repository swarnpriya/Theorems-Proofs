## Naturals
- Naturals are defined as an iductive type in Coq. 
```
Inductive nat : Type :=
  | O : nat
  | S : nat -> nat.
```
nat is a type where Type is the universal type. The two constructors O and S are used to define nat. Nat can be either O
or a succesor of a number. So if we want to write 2 as an inductive nat type. We can write 2 as S(S O).

### Theorem 1: (Proof by structural induction)
x + O = x
Let's do induction on x which gives us two cases to prove.
- Case 1:
O + O = O. This case is trivial to prove as it is computational equality. 
- Case 2:
S x + O = S x. We have x + O = x as IH. Now we replace x with x + O. 
S (x + O) = S x.  
S x = S x. By computational equality. 

### Thorem 2:
(x + y) - y = x 
Lets do inductio 


