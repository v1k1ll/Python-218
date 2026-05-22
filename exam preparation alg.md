## ШПАРГАЛКА В САМОМ НАЧАЛЕ
∧ - and,   
∨ - or,  
≡ - ==,   
¬ - not (букву брать в скобки)  
→ - <=  
0 - ложь  
1 - истина

##
# ВСЕ ЗАДАНИЯ РЕШАЮТСЯ НА САЙТЕ "СДАМ ЕГЭ".  
##
# ТИП - 2
##
1  
№ 28677  
<img width="836" height="215" alt="image" src="https://github.com/user-attachments/assets/33c1ed27-5ef7-4cd1-b811-733df48dedbe" />  
Напишем код для подбора значений
```
print('x y z w')
for x in range(0, 2):
    for y in range(0, 2):
        for z in range(0, 2):
            for w in range(0, 2):
                if ((x <= y) or (y == w)) and ((x or z) == w):
                    print(x,y,z,w)
```
Ответ:zxyw
##
2  
№15124  
<img width="774" height="234" alt="image" src="https://github.com/user-attachments/assets/a8dff25d-5059-405f-8322-2f77072f46ea" />  
```
print('x y z')
for x in range(0, 2):
    for y in range(0, 2):
        for z in range(0, 2):
            if not((x==y) or ((y or z)<=x)):
                print(x,y,z)
```
Ответ:xzy
##
3  
№26974  
<img width="828" height="262" alt="image" src="https://github.com/user-attachments/assets/60ef0b90-30a0-44e1-8ef5-607fc8616c49" />  
```
print('x y z w')
for x in range(0,2):
    for y in range(0,2):
        for z in range(0,2):
            for w in range(0,2):
                if (x or y) and not((y == z))  and not(w):
                    print(x,y,z,w)
```
Ответ:xzyw
##
4  
№15618  
<img width="839" height="224" alt="image" src="https://github.com/user-attachments/assets/6cc472d2-c6f7-4790-91af-e25e41159acd" />  
```
print('x y z w')
for x in range(0,2):
    for y in range(0,2):
        for z in range(0,2):
            for w in range(0,2):
                if not ((x and not (y)) or (y == z) or not (w)):
                    print (x,y,z,w)
```
Ответ:wzyx
##
5  
№15970  
<img width="835" height="254" alt="image" src="https://github.com/user-attachments/assets/639959f1-1741-4c64-934f-61d2d1cfa4df" />  
```
print('x y z w')
for x in range(0, 2):
    for y in range(0, 2):
        for z in range(0, 2):
            for w in range(0, 2):
                if not((x and not(y)) or (y == z) or w):
                    print(x,y,z,w)
```
Ответ:yxwz
##
6  
№18614  
<img width="828" height="252" alt="image" src="https://github.com/user-attachments/assets/2be8a9ae-cccf-49b4-b4a9-2d0e2d06f8d4" />  
чтоб узнать ложную строку
```
print('x y z w')
for x in range(0,2):
    for y in range(0,2):
        for z in range(0,2):
            for w in range(0,2):
                if not (((w <= (not x)) == (z <= y)) and (y or w)):
                    print(x,y,z,w)
```

чтоб узнать истиную строку
```
print('x y z w')
for x in range(0,2):
    for y in range(0,2):
        for z in range(0,2):
            for w in range(0,2):
                if ((w <= (not x)) == (z <= y)) and (y or w):
                    print(x,y,z,w)
```
Ответ:xwyz
##
7  
№55589  
<img width="771" height="327" alt="image" src="https://github.com/user-attachments/assets/73b17767-95dd-4ed3-9e40-e8f4c8653a40" />  
```
print('x y z w f1 f2')
for x in range(0,2):
    for y in range(0,2):
        for z in range(0,2):
            for w in range(0,2):
                f1 = (x <= y) == (w or (not z))
                f2 = (x<=y) and ((not w) == z)
                print(x,y,z,w,int(f1), int(f2))
```
Ответ: xzyw
##
8  
№48423  
<img width="776" height="286" alt="image" src="https://github.com/user-attachments/assets/500f62fb-7e97-4b9a-944e-34c4641db31e" />  
чтоб узнать ложную строку
```
print("x y z w")
for x in range(2):
    for y in range(2):
        for z in range(2):
            for w in range(2):
               if not((x <=(y == w)) and (y == (w <= z))):
                    print(x, y, z, w)
```
чтоб узнать истиную строку
```
print("x y z w")
for x in range(2):
    for y in range(2):
        for z in range(2):
            for w in range(2):
               if (x <=(y == w)) and (y == (w <= z)):
                    print(x, y, z, w)
```
Ответ: yxwz
##
9  
№15787  
<img width="919" height="277" alt="image" src="https://github.com/user-attachments/assets/82326510-d5e4-42f1-b93b-aa7918a632c8" />  
```
print('x y z w')
for x in range(2):
    for y in range(2):
        for z in range(2):
            for w in range(2):
                if not(((x <= y) and (y <= w)) or (z == (x or y))):
                    print(x, y, z, w)
```
Ответ: ywzx
##
10  
№85678  
<img width="879" height="397" alt="image" src="https://github.com/user-attachments/assets/d146adaa-4351-440e-b2bf-792197418611" />
```
print('x y w z')
for x in range (2):
    for y in range (2):
        for w in range (2):
            for z in range (2):
                if not((not w) or ((z <= x) <= y)):
                    print(x,y,w,z)
```
Ответ: yxwz
##
11  
№18578  
<img width="844" height="260" alt="image" src="https://github.com/user-attachments/assets/1e69ee8d-82ca-4d7d-aa89-81ce6bae44ed" />
```
print('x y w z')
for x in range (2):
    for y in range (2):
        for w in range (2):
            for z in range (2):
                if ((x and (not y)) or (w <= z)) == (z == x):
                    print(x,y,w,z)
```
Ответ: zywx
##
12  
№81786  
<img width="873" height="200" alt="image" src="https://github.com/user-attachments/assets/8461b979-f092-4af2-8238-13af1addad09" />
```
print('x y w z')
for x in range (2):
    for y in range (2):
        for w in range (2):
            for z in range (2):
                if (x or y) and (not(y==z)) and (not w):
                    print(x,y,w,z)
```
Ответ: zyxw
##
13  
№17320  
<img width="809" height="213" alt="image" src="https://github.com/user-attachments/assets/7b3649cb-6ff3-4b3c-b5bc-30695bd748c2" />
```

```
Ответ:
##
14  
№48450  

```

```
Ответ:
##
15  
№40718  

```

```
Ответ:
##
16  
№73828  

```

```
Ответ:
##
17  
№45236  
  
```

```
Ответ:
##
18  
№33504  
  
```

```
Ответ:
##
19  
№64932  
  
```

```
Ответ:
##
20  
№64887  
  
```

```
Ответ:
##
21  
№72587  
  
```

```
Ответ:
##
# ТИП - 8
##
1  
№3697   

```

```
Ответ:
##
2  
№78064  

```

```
Ответ:
##
3  
№55625  

```

```
Ответ:
##
4  
№7667  

```

```
Ответ:
##
5  
№17328  

```

```
Ответ:
##
6  
№27539  

```

```
Ответ:
##
7  
№18491  

```

```
Ответ:
##
8  
№37143  

```

```
Ответ:
##
9  
№59745  

```

```
Ответ:
##
10  
№10473  

```

```
Ответ:
##
11  
№60250  

```

```
Ответ:
##
12  
№64938  

```

```
Ответ:
##
13  
№9796  

```

```
Ответ:
##
14  
№27009  

```

```
Ответ:
##
15  
№15822  

```

```
Ответ:
##
16  
№28546  

```

```
Ответ:
##
17  
№15795  
  
```

```
Ответ:
##
18  
№3700  
  
```

```
Ответ:
##
19  
№3237  
  
```

```
Ответ:
##
20  
№13486    
<img width="850" height="64" alt="image" src="https://github.com/user-attachments/assets/27dd1c81-79a3-4bf9-aff3-78017e675baa" />
```
from itertools import *
a=0
for i in product('ABCX', repeat=5):
    if i.count('X') == 1 and (i[0] == 'X' or i[-1] == 'X'):
        a+=1
print(a)
```
Ответ: 162
##
21  
№59741  
  
```

```
Ответ:
##
