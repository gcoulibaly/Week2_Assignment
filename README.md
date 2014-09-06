Week2_Assignment
================
Question#4 Finding numbers that are not divisible by any 3, 7, and 11

> A<-seq(1000) # the sequence of numbers to use
> B<-((A %% 3 !=0)&(A %% 7!=0) & (A %% 11!=0)) # using the boolean operation
> sum(B)         #counting the number of integers that are not divisible by 3, 7, and 11
[1] 520

