# gaurav
#program to check a random number
import random
def prime(x):
    for i in range(2,x):
        if(x%i==0):
            return False
    return True
a=int(input("Enter lower limit: "))
b=int(input("Enter upper limit: "))
x=random.randint(a,b)
print("\n")
print("Range is(%d,%d) a randomlypicked number is %d"%(a,b,x))
if x>0:
    print("%d is positive"%x)
else:
    print("%d is negative"%x)
if (x%2==0):
    print("%d is an even number"%x)
else:
    print("%d is an odd number"%x)


if (prime(x)):
    print("%d is a prime number"%x)
elif(x==1):
    print("1 is neither a prime number nor composite number")
else:
    print("%d is a composite number"%x)

