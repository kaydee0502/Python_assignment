# Python_assignment

## Question 1:
WAP in python to print table of a number up to 12. 
```python
n = int(input())
for i in range(1,11):
    print(i,"x",n,"=",i*n)
        
```
> Output
```
5
1 x 5 = 5
2 x 5 = 10
3 x 5 = 15
4 x 5 = 20
5 x 5 = 25
6 x 5 = 30
7 x 5 = 35
8 x 5 = 40
9 x 5 = 45
10 x 5 = 50
```
## Question 2:
WAP to display all prime numbers up to a given number.
```python
lower = 0 
upper = int(input("Enter upper range: "))  
  
for num in range(lower,upper + 1):  
   if num > 1:  
       for i in range(2,num):  
           if (num % i) == 0:  
               break  
       else:  
           print(num)
```
> Output
```
Enter upper range: 50
2
3
5
7
11
13
17
19
23
29
31
37
41
43
47
```
## Question 3:
WAP to input a number from user and write it in words.
```python
from num2words import num2words

n = int(input("Enter a number : "))
print("In words : ",num2words(n))
```
> Output
```
Enter a number : 521
In words :  five hundred and twenty-one
```
## Question 4:
WAP to define a function which adds arbitrary numbers.
```python

def func(*args):
    print(sum(args))
       
func(2,3,4,9)
```
> Output
```
18
```
## Question 5:
WAP to show the use of keywords arguments in python.
```python
def func(a,b,c):
    print(max(a,b,c))
       
func(c=5,a=6,b=9)
```
> Output
```
9
```
## Question 6:
WAP to show the use of arbitrary keyword arguments in python.
```python
def func(**kwargs):
    for i in kwargs:
        print("key = {} : value = {}".format(i,kwargs[i]))
       
func(b="Kamikaze",a="kaydee",c="blackbess")
```
> Output
```
key = b : value = Kamikaze
key = a : value = kaydee
key = c : value = blackbess
```


## Question 7:
WAP to read a number and print sum of its digits.
```python
n = int(input("enter a number : "))

print("sum of its digits :",sum(map(int,list(str(n)))))
```
> Output
```
enter a number : 89
sum of its digits : 17
```
## Question 8:
WAP to read a list of numbers and print the sun and average.
```python
n = list(map(int,input().split()))
sum_num = sum(n)
print("sum of num is : ",sum_num)
print("average of num is : ",sum_num/2)
```
> Output
```
4 5 6 2 3 9
sum of num is :  29
average of num is :  14.5
```
## Question 9
WAP to read a string from user and print it back after swap case.
```python
s = input("Enter a string ")
print(s.swapcase())
```
> Output
```
Enter a string LmAo
lMaO
```
## Question 10
WAP to read a paragraph from user , calculate number of words, vowels and consonants.
```python
vovels = {"a","e","i","o","u"}

para = input("Enter a paragraph ")

words = para.split()

vovels_count = sum([1 for x in "".join(words) if x in vovels])
consonats_count = len("".join(words))-vovels_count
word_count = len(words)

print("Words count:",word_count)
print("Vovels count:",vovels_count)
print("Consonats count:",consonats_count)

```
> Output
```
Enter a paragraph I am a student of bca fourth sem of jecrc university
Words count: 11
Vovels count: 15
Consonats count: 27
```



