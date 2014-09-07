Week2_Assignment
================
#Question1. Five customers in a line

#1-a) creating vector of five individuals
>queue<-c("James","Mary","Steve", "Alex","Patricia")
> queue
[1] "James"    "Mary"     "Steve"    "Alex"     "Patricia"   #output

#1-b) adding Harold at the end
> queue<-append(queue,"Harold")
> queue
[1] "James"    "Mary"     "Steve"    "Alex"     "Patricia" "Harold"  

#1-c) removing James
> queue<-queue[-1]
> queue
[1] "Mary"     "Steve"    "Alex"     "Patricia" "Harold"  

#1-d) adding Pam in front of Steve
> queue<-append(queue, "Pam",1)
> queue
[1] "Mary"     "Pam"      "Steve"    "Pam"      "Alex"     "Patricia" "Harold"  

#1-e) Removing Harold
> queue<-queue[-7]
> queue
[1] "Mary"     "Pam"      "Steve"    "Pam"      "Alex"     "Patricia"

#1-f) Removing Alex without using index
> queue<-queue[queue !="Alex"]
> queue
[1] "Mary"     "Pam"      "Steve"    "Pam"      "Patricia"

#1-g) looking for Patricia location in the line
> which(queue=="Patricia")
[1] 5

#1-h) counting the number of people
> count<-length(queue)
> count
[1] 5

#Question3 Finding numbers that are not divisible by any 3, 7, and 11

> A<-seq(1000) # the sequence of numbers to use
> B<-((A %% 3 !=0)&(A %% 7!=0) & (A %% 11!=0))        # using the boolean operation
> sum(B)                                             #counting the number of integers that are not divisible by 3, 7, and 11
[1] 520


