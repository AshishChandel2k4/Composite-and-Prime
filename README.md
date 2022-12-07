# Composite-and-Prime
a=int(input("Enter first number:"))
b=int(input("Enter last number:"))
count=0
count1=0
count2=0
for i in range(a,b+1):
    if(i ==1):
        continue
    count2=1
    for j in range(2,i):
        if(i%j==0):
            count2=0
            count=count+1
            break
    if (count2==1):
        print(i,"is Prime Number")
        count1=count1+1
    else:
        print(i,"is Composite Number")
print(count,"Prime Numbers and",count1,"Composite Number")
