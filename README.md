# 1

names = ["khaled", "omar", "Ahmed"]
for n in names:
    print(n, len(n), sep='-')



#2

print("Enter two equal in length lists:")

arr1 = list(map(int, input().split()))
arr2 = list(map(int, input().split()))

res = []

for i in range(len(arr1)):
    if arr1[i] not in arr2:
        res.append(arr1[i])
    if arr2[i] not in arr1:
        res.append(arr2[i])

print(res)



#3

std = {"name": "khaled", "Age": 21}
std.update({"hoppy": "Football"})

print(std.get("name"), std.get("Age"))
print(std)

for key, val in std.items():
    print(f"the {key} is {val}")




#4

print("Enter two strings:")

def ok(s1, s2):
    mnlen = min(len(s1), len(s2))
    ok = True

    if len(s1) >= len(s2):
        for i in range(mnlen):
            if s2[i] not in s1:
                ok = False
                break
    else:
        for i in range(mnlen):
            if s1[i] not in s2:
                ok = False
                break
    return ok

a = input().strip()
b = input().strip()

print("YES" if ok(a, b) else "NO")




#5

n = 9
while True:
    num = int(input("Guess a number from 1 to 10: "))
    if num == n:
        print("congratulation")
        break



#6

s = input("Enter a string: ").strip()
rev = s[::-1]

if(s == rev):
    print("isPalindrome")
else:
    print("notPalindrome")# taskpaython1
