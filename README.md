'''
1
a=int(input("Enter 100 ruppees notes : "))
b=int(input("Enter 500 ruppees notes: "))
c=int(input("Enter 1000 ruppees notes: "))
print("Total amount : ",(a*100)+(b*500)+(c*1000))
'''
'''
2
a=int(input("Enter hours : "))
if(a>=1 and a<=23):
    c=a*20
    print("Total bill is : ",c)
elif(a<1):
    b=10
    print("Total bill is : ",b)
else:
    d=100
    print("Total bill is : ",d)
'''
'''
3
t=(input("Enter temperature : "))
p=(input("Enter humididty : "))
if(t=="Warm"):
    if(p=="Dry"):
        print("Play Basketball")
    elif(p=="Humid"):
        print("Play Tennis")
elif(t=="Cold"):
    if(p=="Dry"):
        print("Play Cricket")
    elif(p=="Humid"):
        print("Swim")
'''
'''
4
a=[]
for i in range(1,6):
    b=int(input("Enter chocolate cost : "))
    a.append(b)
c=[ele*7 for ele in a] 
print(sum(c))
'''

'''
5)a
import math
x=int(input("Enter x value : "))
n=int(input("Enter n value : "))
sum=0
i=1
while i<=n:
    sum=sum+(math.pow(x,i)/math.factorial(i))
    i=i+1;
print(sum)
5)b
import math
x=int(input("Enter x value : "))
n=int(input("Enter n value : "))
sum=0
i=0
while i<=n:
    sum=sum+math.pow(x,i)
    i=i+1
print(sum)
'''

'''
6

def dec_bin(num):
    print(bin(num)[2:])
n=int(input("Enter a number : "))
dec_bin(n)
'''
'''
7
def Calc_GCD_Recurr(a,b):
    if(b==0):
        return a
    else:
        return Calc_GCD_Recurr(b,a%b)
a=int(input("Enter value of a : "))
b=int(input("Enter value of b : "))
print("The gcd is ",Calc_GCD_Recurr(a,b))
'''
'''
8
------------without recursion
l=[]
b=int(input("Enter a number: "))
while(b>0):
    dig=b%10
    l.append(dig)
    b=b//10
print("Sum is:")
print(sum(l))
-----with recursion
def sumo( n ):
    if n == 0:
        return 0
    return (n % 10 + sumo(int(n / 10)))
num = int(input("Enter a number : "))
r=sumo(num)
print("Sum of digit is ", r)
'''
'''
9
s=input("Enter a string : ")
u=0
l=0
for i in s:
    if(i.isupper()):
        u=u+1
    elif(i.islower()):
        l=l+1
print("Lower count : ",l)
print("Upper count : ",u)
'''
'''
10
def startEndVowels(word):
    s="AaEeIiOoUu"
    if s.__contains__(word[0]) and s.__contains__(word[-1]) :
        return True
    else :
        return False
s=input("Enter a word : ")
if startEndVowels(s):
    print("Given word ",s,"starts and ends with Vowel")
else :
    print("Given word ", s, "not starts and ends with Vowel")
'''
