# hshs
haskell in scheme  
gauche

example:
```
(define fact (hshs  
"f 0 = 1  
f n = n * f (n - 1)  
"))  
(print (fact 4)) ;24
```

example: list
```
(define haskell-map (hshs
"m _ [] = []
m f (x:y) = f x : m f y
"))
(equal? (map even? '(0 1 2 3 4))
        ((haskell-map even?) '(0 1 2 3 4))) ; => #t
```
