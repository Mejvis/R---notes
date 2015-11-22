7: Matrices and Data Frames  

> my_vector<-1:20  

> my_vector
 [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20  

> dim(my_vector)
NULL  

> length(my_vector)
[1] 20  

> dim(my_vector) <- c(4, 5)  

> dim(my_vector)
[1] 4 5  

> attributes(my_vector)
$dim
[1] 4 5  

> my_vector
     [,1] [,2] [,3] [,4] [,5]
[1,]    1    5    9   13   17
[2,]    2    6   10   14   18
[3,]    3    7   11   15   19
[4,]    4    8   12   16   20  

> class(my_vector)
[1] "matrix"  

> my_matrix <- my_vector  

> my_matrix2 <- matrix(1:20, 4, 5)  

> identical(my_matrix, my_matrix2)
[1] TRUE
  
> patients <- c("Bill", "Gina", "Kelly", "Sean")  

> cbind(patients, my_matrix)
     patients                       
[1,] "Bill"   "1" "5" "9"  "13" "17"
[2,] "Gina"   "2" "6" "10" "14" "18"
[3,] "Kelly"  "3" "7" "11" "15" "19"
[4,] "Sean"   "4" "8" "12" "16" "20"  

> my_data <- data.frame(patients, my_matrix)  

> my_data
  patients X1 X2 X3 X4 X5
1     Bill  1  5  9 13 17
2     Gina  2  6 10 14 18
3    Kelly  3  7 11 15 19
4     Sean  4  8 12 16 20  

> class(my_data)
[1] "data.frame"
  
  
> cnames <- c("patient", "age", "weight", "bp", "rating", "test")  

> colnames(my_data) <- cnames  

> my_data
  patient age weight bp rating test
1    Bill   1      5  9     13   17
2    Gina   2      6 10     14   18
3   Kelly   3      7 11     15   19
4    Sean   4      8 12     16   20  


