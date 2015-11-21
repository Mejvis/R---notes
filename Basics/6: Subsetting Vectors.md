6: Subsetting Vectors

> x
 [1] -0.14166341  0.04530465          NA  0.38077358  0.51892699  1.31545065  0.69825656          NA          NA -0.25097625          NA          NA
[13] -0.50175931 -1.04913569          NA  0.59345863  0.29992913 -0.04214013  0.18220145          NA          NA          NA  1.10834108          NA
[25]  0.84242149          NA  0.06728923  0.66230777          NA  0.03987666          NA          NA -1.50532124          NA          NA          NA
[37]          NA          NA -0.32019667          NA


> x[1:10]
 [1] -0.14166341  0.04530465          NA  0.38077358  0.51892699  1.31545065  0.69825656          NA          NA -0.25097625  
 
 | What do you think x[is.na(x)] will give you?

1: A vector of length 0
2: A vector of all NAs
3: A vector with no NAs
4: A vector of TRUEs and FALSEs

Selection: 2  

> x[is.na(x)]
 [1] NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA  
 
 > y <- x[!is.na(x)]  
 
 > y
 [1] -0.14166341  0.04530465  0.38077358  0.51892699  1.31545065  0.69825656 -0.25097625 -0.50175931 -1.04913569  0.59345863  0.29992913 -0.04214013
[13]  0.18220145  1.10834108  0.84242149  0.06728923  0.66230777  0.03987666 -1.50532124 -0.32019667  

| Recall that the expression y > 0 will give us a vector of logical values the same length as y, with TRUEs corresponding to values of y that are
| greater than zero and FALSEs corresponding to values of y that are less than or equal to zero. What do you think y[y > 0] will give you?

1: A vector of all the negative elements of y
2: A vector of TRUEs and FALSEs
3: A vector of all the positive elements of y
4: A vector of length 0
5: A vector of all NAs

Selection: 3  


> y[y>0]
 [1] 0.04530465 0.38077358 0.51892699 1.31545065 0.69825656 0.59345863 0.29992913 0.18220145 1.10834108 0.84242149 0.06728923 0.66230777 0.03987666  
 
 > x[x>0]
 [1] 0.04530465         NA 0.38077358 0.51892699 1.31545065 0.69825656         NA         NA         NA         NA         NA 0.59345863 0.29992913
[14] 0.18220145         NA         NA         NA 1.10834108         NA 0.84242149         NA 0.06728923 0.66230777         NA 0.03987666         NA
[27]         NA         NA         NA         NA         NA         NA         NA  


> x[!is.na(x) & x >0]
 [1] 0.04530465 0.38077358 0.51892699 1.31545065 0.69825656 0.59345863 0.29992913 0.18220145 1.10834108 0.84242149 0.06728923 0.66230777 0.03987666  

> x[c(3, 5, 7)]
[1]        NA 0.5189270 0.6982566  


| It's important that when using integer vectors to subset our vector x, we stick with the set of indexes {1, 2, ..., 40} since x only has 40 elements.
| What happens if we ask for the zeroth element of x (i.e. x[0])? Give it a try.

> x[0]
numeric(0)  

> x[3000]
[1] NA  

> x[c(-2, -10)]
 [1] -0.14166341          NA  0.38077358  0.51892699  1.31545065  0.69825656          NA          NA          NA          NA -0.50175931 -1.04913569
[13]          NA  0.59345863  0.29992913 -0.04214013  0.18220145          NA          NA          NA  1.10834108          NA  0.84242149          NA
[25]  0.06728923  0.66230777          NA  0.03987666          NA          NA -1.50532124          NA          NA          NA          NA          NA
[37] -0.32019667          NA  


> x[-c(2, 10)]
 [1] -0.14166341          NA  0.38077358  0.51892699  1.31545065  0.69825656          NA          NA          NA          NA -0.50175931 -1.04913569
[13]          NA  0.59345863  0.29992913 -0.04214013  0.18220145          NA          NA          NA  1.10834108          NA  0.84242149          NA
[25]  0.06728923  0.66230777          NA  0.03987666          NA          NA -1.50532124          NA          NA          NA          NA          NA
[37] -0.32019667          NA  

> vect <- c(foo = 11, bar = 2, norf = NA)  

> vect
 foo  bar norf 
  11    2   NA   


> names(vect)
[1] "foo"  "bar"  "norf"  

> vect2 <- c(11, 2, NA)  
 
> names(vect2) <- c("foo", "bar", "norf") 

> identical(vect, vect2)
[1] TRUE  

| If we want the element named "bar" (i.e. the second element of vect), which command would get us that?

1: vect["2"]
2: vect[bar]
3: vect["bar"]

Selection: 3

> vect["bar"]
bar 
  2  

> vect[c("foo", "bar")]
foo bar 
 11   2 




 



