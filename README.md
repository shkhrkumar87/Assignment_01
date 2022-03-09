# Assignment_01
# 1.Check wether given number is even or not
n = int(input())
if n%2==0:
  print("Even")
else:
  print("Not even")
 
 
 

 # 2.Convert temperature in degree centigrade to Fahrenhit
c =int(input())
f =(c*9/5)+32
print(f)





 # 3. Product of real numbers
from functools import reduce
real_numbers = []
n = int(input())
for i in range(n):
  num =int(input())
  real_numbers.append(num)
product=reduce((lambda x,y:x*y),real_numbers)
print(product)


# 4. Factorial of numbers
def fact(n):
 if n==0:
    return 1
 else:
    return n*fact(n-1)
m= int(input())
res = fact(m)
print(res)

# 5. Linear search
def ls(l1, x):
   for i in range(len(l1)):
      if l1[i] == x:
         return i
   return "Not Found"
l1 = ['t','u','t','o','r','i','a','l']
x = 'o'
print("element found at index "+str(ls(l1,x)))


# 6. Binary search
 def binary_search(arr, low, high, x):
    if high >= low:
        mid = (high + low) // 2
        if arr[mid] == x:
            return mid
        elif arr[mid] > x:
            return binary_search(arr, low, mid - 1, x)
        else:
            return binary_search(arr, mid + 1, high, x)
    else:
        return -1
arr = [ 2, 3, 4, 10, 40 ]
x = 3
result = binary_search(arr, 0, len(arr)-1, x)
if result != -1:
    print("Element is present at index", str(result))
else:
    print("Element is not present in array")
    
    
 # 7. Largest Value
 l1 = []
le= int(input("Enter the length of the array l1       :       "))
for i in range(le):
  e = int(input("Enter the all element     :                   "))
  l1.append(e)
l1.sort()
print("Array l1  =",   l1)
print("Largest element is:", l1[-1])



 # 8. Python program to delete an element from a list by index
list = [1,2,3,4,5,6,7,8,9]
del list[3]
print(list)

 # 9.Python program to print all the items in a dictionary
 dicta = {'mango':50, 'apple':90,'Goa':40,'fineapple':60}
[print(value) for value in dicta.values()]



# 10.Sum and average of 10 numbers
sum=0
num1=int(input("please enter the 10 integers      :    "))
for i in range(1,num1+1,1):
  num= int(input("enter the number    :                "))
  sum = sum+num
print("sum  =   ",sum)
print("average   =    ",sum/num1)



