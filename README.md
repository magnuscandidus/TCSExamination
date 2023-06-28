# TCSExamination
for t in range(int(input())):
    x1, y1, z1 = map(int, input().split())
    x2, y2, z2 = map(int, input().split())
    s1 = x1+y1+z1
    s2 = x2+y2+z2
    if s1>s2:
        print("Dragon")
    elif s2>s1:
        print("Sloth")
    elif (s1==s2 and x1>x2) or (s1==s2 and x1==x2 and y1>y2):
        print("Dragon")
    elif (s1==s2 and x2>x1) or (s1==s2 and x1==x2 and y2>y1):
        print("Sloth")
    else:
        print("Tie")
    
