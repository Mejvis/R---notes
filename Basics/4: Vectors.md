4: Vectors

num_vect<-c(0.5, 55, -10, 6)  
tf <- num_vect<1  

> tf
[1]  TRUE FALSE  TRUE FALSE  

> num_vect >= 6
[1] FALSE  TRUE FALSE  TRUE  

The `<` and `>=` symbols in these examples are called 'logical operators'. Other logical operators include `>`, `<=`, `==` for exact equality, and
`!=` for inequality.  

| If we have two logical expressions, A and B, we can ask whether at least one is TRUE with A | B (logical 'or' a.k.a. 'union') or whether they are both
| TRUE with A & B (logical 'and' a.k.a. 'intersection'). Lastly, !A is the negation of A and is TRUE when A is FALSE and vice versa.

> my_char <- c("My", "name", "is")  

> my_char
[1] "My"   "name" "is"  

> paste(my_char, collapse = " ")
[1] "My name is"  

> my_name<-c(my_char, "Matt")

> my_name
[1] "My"   "name" "is"   "Matt"  

> paste(my_name, collapse = " ")
[1] "My name is Matt"  

> paste("Hello", "world!", sep = " ")
[1] "Hello world!"  

> paste(1:3, c("X", "Y", "Z"), sep = "")
[1] "1X" "2Y" "3Z"  

> paste(LETTERS, 1:4, sep = "-")
 [1] "A-1" "B-2" "C-3" "D-4" "E-1" "F-2" "G-3" "H-4" "I-1" "J-2" "K-3" "L-4" "M-1" "N-2" "O-3" "P-4" "Q-1" "R-2" "S-3" "T-4" "U-1" "V-2" "W-3" "X-4"
[25] "Y-1" "Z-2"  

