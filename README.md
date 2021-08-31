# divisible-numbers-in-fib-terms
#code to print the number of numbers in a fibonacci series divisible by a particular integer .
n = int(input())
#the number of terms in series you want 
m = int(input())
#the number you want to check the integers in the series are divisible by
a = 0
b = 1
fib_term = 0
count = 1
series = []
even = []

while(count <= n):
  series.append(fib_term)
  count += 1
  a = b
  b = fib_term
  fib_term = a + b
  
for x in series:
    if x%m == 0:
        even.append(x)
        
print(sum(even))
        
  
