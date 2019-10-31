# python_refund
couresa

# 第三週3.1

x1 = int(input())
x2 = int(input())
y = int(input())
if  x1 - y <= 0:
     x2 += x1
     x1 = 0
else:  
    x1 -= y
    x2 += y

print(str(x1) + " " + str(x2))

# 第三週3.2找錢機

a = int(input())
u = (1000-a)//500
v = (1000-a -500 * u)//100
w = (1000-a -500 * u -100 * v)//50
x = (1000-a -500 * u -100 * v - 50 * w )//10
y = (1000-a -500 * u -100 * v - 50 * w-10 * x )//5
z = (1000-a -500 * u -100 * v - 50 * w-10 * x - 5* y )

b = str()

if u > 0:
   b += str(500) + ", " +str(u)
if v > 0:
   if b:
       b += "; " 
   b += str(100) + ", " +str(v)
if w > 0:
   if b:
      b += "; " 
   b += str(50) + ", " +str(w)
if x > 0:
   if b:
      b += "; "
   b += str(10) + ", " +str(x)
if y > 0:
   if b:
      b += "; "
   b += str(5) + ", " +str(y) 
if z > 0:
   if b:
      b += "; "
   b += str(1) + ", " +str(z)   

print(b)
