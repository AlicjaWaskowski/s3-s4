# s3-s4

#s3
> s <- list(Name = my_data$Name, Age = my_data$Age, GPA = my_data$GPA, Major = my_data$Major)
> print(s)
$Name
[1] "Michael" "John"    "David"  

$Age
[1] 23 25 22

$GPA
[1] 3.9 3.6 3.7

$Major
[1] "Engineering" "Economics"   "Finance"  

#s4
> setClass("student", 
+          slots = list(
+            Name = "character", 
+            Age = "numeric", 
+            GPA = "numeric", 
+            Major = "character"
+          ))
> s4 <- new("student", Name = my_data$Name, Age = my_data$Age, GPA = my_data$GPA, Major = my_data$Major)
> s4
An object of class "student"
Slot "Name":
[1] "Michael" "John"    "David"  

Slot "Age":
[1] 23 25 22

Slot "GPA":
[1] 3.9 3.6 3.7

Slot "Major":
[1] "Engineering" "Economics"   "Finance"    
