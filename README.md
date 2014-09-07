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

Question5
#checking the pythagorean theorem
> pythagore<-function(a,b,c){
+ d<-a^2 +b^2
+ k<-b^2 + a^2
+ if ((d==c*c)&&(k==c*c)&&(c*c==d)&&(c*c==k)) print"Yes, it is a right triangle"
Error: unexpected string constant in:
"k<-
if ((d==c*c)&&(k==c*c)&&(c*c==d)&&(c*c==k)) print"Yes, it is a right triangle""
> if ((d==c*c)&&(k==c*c)&&(c*c==d)&&(c*c==k)) print"Yes, it is a right triangle")
Error: unexpected string constant in "if ((d==c*c)&&(k==c*c)&&(c*c==d)&&(c*c==k)) print"Yes, it is a right triangle""
> #checking the pythagorean theorem
> pythagore<-function(a,b,c){
+ d<-a^2 +b^2
+ k<-b^2 + a^2
+ if ((d==c*c)&&(k==c*c)&&(c*c==d)&&(c*c==k)) print("Yes, it is a right triangle")
+ else print("No, it is not a right triangle")
+ }
> f(3,4,5)
Error: could not find function "f"
> pythagore(3,4,5)
[1] "Yes, it is a right triangle"
> pythagore(4,3,5)
[1] "Yes, it is a right triangle"
> pythagore(4,5,3)
[1] "No, it is not a right triangle
