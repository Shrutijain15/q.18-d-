# Q.18-d-
def fibonacci(n)
  if n<=0:
    return []
  elif n==1:
    return[0]
  elif n==2:
    return[0,1]
  else :
     fib =fibonacci (n-1)
     fib.apend (fib[-1] + fib[-2])
     return fib

n= int(input("enter the number of terms:"))     
print("the first {} term of the fibonacci series are:".format (n))
print(fibonacci (n))
