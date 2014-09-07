Week2_Assignment
================
Question#4 Finding numbers that are not divisible by any 3, 7, and 11

> A<-seq(1000) # the sequence of numbers to use
> B<-((A %% 3 !=0)&(A %% 7!=0) & (A %% 11!=0)) # using the boolean operation
> sum(B)         #counting the number of integers that are not divisible by 3, 7, and 11
[1] 520

Question#1-a) create a vector with 5 names
> queue<-c("James", "Mary", "Steve", "Alex", "Paticia")
> queue
[1] "James"   "Mary"    "Steve"   "Alex"    "Paticia"

>Question# 1-b)  adding new name
> queue<-append(queue, "Harold",5)
> queue
[1] "James"   "Mary"    "Steve"   "Alex"    "Paticia" "Harold" 

Question#1-c) Removing the first element in a list
> queue[-1]
[1] "Mary"    "Steve"   "Alex"    "Paticia" "Harold" 
> 
