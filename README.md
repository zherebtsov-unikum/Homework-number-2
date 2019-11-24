from random import random
N = 5
a = []
b = []
c = []
for i in range(N):
    z = []
    for j in range(N): 
        n = int(random() * 100)
        z.append(n) 
        print("%4d" % n, end='') 
    print() 
    a.append(z) 
print()


for i in range(N):
    z = []
    for j in range(N):
        n = int(random() * 100)
        z.append(n)
        print("%4d" % n, end='')
    print()
    b.append(z)
print()

for i in range(N):
    z = []
    for j in range(N):
        if a[i][j] > b[i][j]:
            n = a[i][j]
        else:
            n = b[i][j]
        z.append(n)
    c.append(z)
print()


for i in range(N):
    for j in range(N):
        n = c[i][j]
        print("%4d" % n, end='')
    print()
