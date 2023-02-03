# assignment-2
assignement 2
Bhargavi Chukkapalli (700743393)
https://drive.google.com/file/d/1gs32ibvXtMXUj9yzasIvigUQ4NzMWVlk/view?usp=sharing
code documentation
1.. Use a python code to display the following star pattern using the for loop
   n = int(input())  ##taken an input from the user ,to know how many rows need's to be printed
   l = [] 
   for i in range(1,n+1):   ## this for loop is to print the pattern in forward (increasing stars with the row)
       l.append("*"*i)  
   for i in range(n-1,0,-1): ## (this for loop is to print the pattern in backward (decreasing no of stars with the row) ..both the for loops varies with the range function)
       l.append("*"*i)
   print("\n".join(l))


2..#2.Use looping to output the elements from a provided list present at odd indexes.
my_list = [10, 20, 30, 40, 50, 60, 70, 80, 90, 100]  ##given list
for i in range(1,len(my_list)+1,+2):    ## for loop to print the elements in the odd position of list 
    print(my_list[i])
    
3..#3.Write a code that appends the type of elements from a given list.
x = [23, 'Python', 23.98]
l1=[]
for i in range(0,len(x)):   ## type() function is used to find the type of an element, and append() is used to add element to the list 
    l1.append(type(x[i]))
print(x)
print(l1)

4..#4.. Write a function that takes a list and returns a new list with unique items of the first list.
n1 = int(input("Enter no. the elements of the list"))
l2= []
for i in range(0,n1):   ## used to input the list elements from the user
    element = int(input())
    l2.append(element)
s=set(l2)   ## set will not have duplicate elements so to find the unique elements of the list , converted the existing list to set
print(sorted(s))


5..#5.Write a function that accepts a string and calculate the number of upper-case letters and lower-case letters.
def string_function(s):         ## created a string function 
    diction={"UPPER_CASE":0, "LOWER_CASE":0}   ## and a dictionary with keys uppercase and lowercase
    for i in s:
        if i.isupper():        ## is used to check whether the letter is uppercase or not
           diction["UPPER_CASE"]+=1
        elif i.islower():       ## is used to check whether the letter is lowercase or not
           diction["LOWER_CASE"]+=1
        else:
           pass
    print ("No. of Upper case characters : ", diction["UPPER_CASE"])
    print ("No. of Lower case Characters : ", diction["LOWER_CASE"])

string_function('The quick Brow Fox')
    
