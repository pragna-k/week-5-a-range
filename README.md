# week-5-a-range
n<-scan()
big=n[1]
small=n[1]
for(i in 1:length(n)){
  if(n[i]>big){
    big=n[i]
  }
}
for(i in 1:length(n)){
  if(n[i]<small){
    small=n[i]
  }
}
sprintf("Big value is %d",big)
sprintf("Small value is %d",small)
range=big-small
sprintf("Range of the given values is %d",range)


OUTPUT:
1: n<-scan()
Error in scan() : scan() expected 'a real', got 'big=n[1]'
> n<-scan()
1: 1
2: 3
3: 5
4: 9
5: 7
6: 6
7: 4
8: 2
9: 8
10: 
Read 9 items
> big=n[1]
> small=n[1]
> for(i in 1:length(n)){
+   if(n[i]>big){
+     big=n[i]
+   }
+ }
> for(i in 1:length(n)){
+   if(n[i]<small){
+     small=n[i]
+   }
+ }
> sprintf("Big value is %d",big)
[1] "Big value is 9"
> sprintf("Small value is %d",small)
[1] "Small value is 1"
> range=big-small
> sprintf("Range of the given values is %d",range)
[1] "Range of the given values is 8"
> 
 


#Range
print("enter data")
n <- scan()
print(n)
for(i in 1:(length(n)-1)){
  for(j in (i+1):length(n)){
    if(n[i] > n[j]){
      n[c(i,j)]=n[c(j,i)]
    }
  }
}
print(paste("Largest number",n[length(n)]))
print(paste("Samllest number",n[1]))
range=n[length(n)]-n[1]
print("The measure of dispersion Range :")
print(range)



OUTPUT:
> #Range
> print("enter data")
[1] "enter data"
> n <- scan()
1: 1
2: 2
3: 4
4: 15
5: 9
6: 8
7: 7
8: 5
9: 
Read 8 items
> print(n)
[1]  1  2  4 15  9  8  7  5
> for(i in 1:(length(n)-1)){
+   for(j in (i+1):length(n)){
+     if(n[i] > n[j]){
+       n[c(i,j)]=n[c(j,i)]
+     }
+   }
+ }
> print(paste("Largest number",n[length(n)]))
[1] "Largest number 15"
> print(paste("Samllest number",n[1]))
[1] "Samllest number 1"
> range=n[length(n)]-n[1]
> print("The measure of dispersion Range :")
[1] "The measure of dispersion Range :"
> print(range)
[1] 14
> 
> 
