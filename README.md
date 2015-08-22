# hshs
haskell in scheme  
gauche

example1:  
```
(define fact (hshs  
"f 0 = 1  
f n = n* f (n - 1)  
"))  
(print (fact 4)) ;24
```

example2: curry  
```
(define add (hshs  
"f a b c = a+b+c  
"))  
(define add-1 (add 1))  
(define add-1+2 (add-1 2))  
(define add-1+2+3 (add-1+2 3))  
(print add-1+2+3) ;6
```
