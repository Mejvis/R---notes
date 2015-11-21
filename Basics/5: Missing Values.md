5: Missing Values

> x<- c(44, NA, 5, NA)  

> x*3
[1] 132  NA  15  NA  

> y<- rnorm(1000) - a vector containing 1000 draws from a standard normal distribution with y <- rnorm(1000)  

> z<- rep(NA, 1000)  

> my_data <- sample(c(y, z), 100)  

> my_na <- is.na(my_data)  

> my_na
  [1] FALSE  TRUE  TRUE FALSE  TRUE FALSE FALSE FALSE  TRUE FALSE FALSE  TRUE  TRUE  TRUE  TRUE FALSE FALSE FALSE  TRUE FALSE  TRUE FALSE FALSE  TRUE
 [25]  TRUE FALSE  TRUE FALSE  TRUE FALSE FALSE  TRUE  TRUE FALSE FALSE  TRUE  TRUE FALSE FALSE  TRUE FALSE FALSE  TRUE  TRUE  TRUE  TRUE FALSE  TRUE
 [49]  TRUE FALSE  TRUE FALSE  TRUE FALSE  TRUE  TRUE  TRUE FALSE FALSE FALSE  TRUE  TRUE  TRUE  TRUE  TRUE  TRUE  TRUE  TRUE FALSE  TRUE  TRUE  TRUE
 [73] FALSE  TRUE  TRUE  TRUE  TRUE FALSE FALSE  TRUE  TRUE FALSE FALSE FALSE FALSE FALSE FALSE  TRUE  TRUE  TRUE FALSE  TRUE FALSE FALSE FALSE FALSE
 [97] FALSE  TRUE  TRUE  TRUE  
 
 
 > my_data == NA
  [1] NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA
 [50] NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA
 [99] NA NA  
 
 > sum(my_na)
[1] 54  

> my_data
  [1]  0.567094589           NA           NA -0.854952041           NA  0.214773132  0.469090553 -0.101531108           NA  1.771288439 -0.478758135
 [12]           NA           NA           NA           NA -0.798001878  0.625666538 -0.220285790           NA  0.157205757           NA  0.513134679
 [23] -0.382361575           NA           NA  0.030556006           NA  1.308944596           NA -0.820495056  0.804955532           NA           NA
 [34]  0.494340331  1.928952680           NA           NA  0.567552207  0.517719750           NA -0.513148335 -1.854042510           NA           NA
 [45]           NA           NA -0.838646692           NA           NA  0.004977517           NA -1.652967332           NA -0.158381000           NA
 [56]           NA           NA  1.031870453  1.029098120  0.040919112           NA           NA           NA           NA           NA           NA
 [67]           NA           NA  0.769171587           NA           NA           NA -0.165318616           NA           NA           NA           NA
 [78]  0.436421091 -0.380249789           NA           NA  0.696587065  1.232133818 -0.477539112 -0.535469245  0.321582501 -0.344495254           NA
 [89]           NA           NA -1.374942765           NA  0.150342545  0.466119400 -0.102905202 -0.279993744  1.315660362           NA           NA
[100]           NA  

> 0/0
[1] NaN  

> Inf-Inf
[1] NaN  
