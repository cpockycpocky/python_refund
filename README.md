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
