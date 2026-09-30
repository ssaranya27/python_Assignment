# python_Assignment


'''1.	Print all prime numbers between input range (Ex – input 20 50, prints all prime numbers between 20 and 50).'''
```
def isPrime(n):
    if n<2:
        return False
    for i in range(2,int(n**0.5) + 1):
        if n%i==0:
            return False
    return True
def printPrime():
    n=int(input())
    m=int(input())
    for i in range(n,m+1):
        if(isPrime(i)):
            print(i,end=" ")
printPrime()
```

'''2.	Factorial using recursion'''
```
def fact(n):
    if n==1:
        return 1
    return n*fact(n-1)

n=int(input())
result=fact(n)
print("The factorial of",n,"is",result)
```

'''3.	Square of numbers using lambda'''
```
n=int(input())
square=lambda n:n*n
print("Square of number:",square(n))
```

'''4.	Find the second largest element in a list'''
```
lis=list(map(int,input().split()))
largest=lis[0]
second_largest=float('-inf')
for i in range(1,len(lis)):
    if lis[i] > largest:
        second_largest=largest
        largest=lis[i]
    elif largest<lis[i]<second_largest:
        second_largest=lis[i]
print("The second largest element in the list:",second_largest)

```

'''5.	Count frequency of characters in a string'''
```
word=input()
freq={}
for i in word:
    freq[i]=freq.get(i,0)+1
print(freq)
```

'''6.	Calculate area of a circle using math library.'''
```
import math
radius=int(input())
print("The area of the circle is",(radius*radius*math.pi).__round__(2))
```

'''7.	Reverse a string without using built‑in reverse'''
```
word=input()
print("The reverse string is",word[::-1])

```
'''8.	Remove duplicates from a list'''
```
duplicate_list = list(map(int, input().split()))

seen = set()
unique_list = []

for i in duplicate_list:
    if i not in seen:
        unique_list.append(i)
        seen.add(i)

print("Before removing duplicates:", duplicate_list)
print("After removing duplicates:", unique_list)
```

    '''9.	Merge two dictionaries'''
```
d1 = {'a': 10, 'b': 20}
d2 = {'a': 30, 'd': 40}

d1.update(d2)

print(d1)

```
'''10.	Fibonacci series using recursion'''
```
def fib(n):
    if n <= 1:
        return n
    return fib(n-1) + fib(n-2)

n = int(input("Enter number of terms: "))
```

for i in range(n):
    print(fib(i), end=" ")

