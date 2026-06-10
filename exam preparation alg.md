# ШПАРГАЛКИ
# 2.  
∧ - and,   
∨ - or,  
≡ - ==,   
¬ - not (букву брать в скобки)  
→ - <=  
0 - ложь  
1 - истина
----------------      
# 8.  
### from itertools import * - из intertool импортировать всё  
### product('...', repeat=...) - все комбинации указанных букв в указанном порядке ('Буквы', кол-во букв в строке)
### for i in permutations('', r=...) - все комбинации указанных букв без повторений одиноковых букв ('Буквы', кол-во букв в строке)

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
print('x y w z')
for x in range (2):
    for y in range (2):
        for w in range (2):
            for z in range (2):
                if ((x and y) or (y and z)) == ((x <= w) and (w <=z)):
                    print(x,y,w,z)
```
Ответ: xwzy
##
14  
№48450  
<img width="845" height="218" alt="image" src="https://github.com/user-attachments/assets/dd2dd081-9b30-46f3-b9fd-9337627dfa26" />
чтоб узнать ложную строку
```
print('x y w z')
for x in range (2):
    for y in range (2):
        for w in range (2):
            for z in range (2):
                if not ((w <= (y == z)) and (y == (z <=x))):
                    print(x,y,w,z)
```
чтоб узнать истиную строку
```
print('x y w z')
for x in range (2):
    for y in range (2):
        for w in range (2):
            for z in range (2):
                if (w <= (y == z)) and (y == (z <=x)):
                    print(x,y,w,z)
```
Ответ: zwyx
##
15  
№40718  
<img width="841" height="208" alt="image" src="https://github.com/user-attachments/assets/2a4bd183-47b8-48b3-aeb3-3cd6caf68201" />
```
print('x y w z')
for x in range (2):
    for y in range (2):
        for w in range (2):
            for z in range (2):
                if not (((x <= y) and (z or w)) <= ((x == w) or (y and (not z)))):
                    print(x,y,w,z)
```
Ответ: yxwz
##
16  
№73828  
<img width="752" height="197" alt="image" src="https://github.com/user-attachments/assets/497da220-13ae-4eae-aa70-ba57c0f072e8" />
чтоб узнать ложную строку
```
print('x y w z')
for x in range (2):
    for y in range (2):
        for w in range (2):
            for z in range (2):
                if not ((x == (y <= z)) and (y == (not(z <=w)))):
                    print(x,y,w,z)
```
чтоб узнать истиную строку
```
print('x y w z')
for x in range (2):
    for y in range (2):
        for w in range (2):
            for z in range (2):
                if (x == (y <= z)) and (y == (not(z <=w))):
                    print(x,y,w,z)
```
Ответ: wzxy
##
17  
№45236  
<img width="851" height="215" alt="image" src="https://github.com/user-attachments/assets/be1149c8-b0db-4658-9ecb-da19839c087f" />
```
print('x y w z')
for x in range (2):
    for y in range (2):
        for w in range (2):
            for z in range (2):
                if not((not(x <= w)) or (y == z) or y):
                    print(x,y,w,z)
```
Ответ: zxwy
##
18  
№33504  
<img width="836" height="206" alt="image" src="https://github.com/user-attachments/assets/40a03c7d-04ec-4f62-8455-8013f43e989d" />
```
print('x y w z')
for x in range (2):
    for y in range (2):
        for w in range (2):
            for z in range (2):
                if not (((x == (not y)) <= (y and (not z))) or (z and (not w))):
                    print(x,y,w,z)
```
Ответ: wzxy
##
19  
№64932  
<img width="745" height="191" alt="image" src="https://github.com/user-attachments/assets/0c4d80e6-4cb7-408b-9806-48082fbd6c32" />
```
print('x y w z')
for x in range (2):
    for y in range (2):
        for w in range (2):
            for z in range (2):
                if ((x ==z) <= ((not y) or w)) == (not((w <= z) or (x<= y))):
                    print(x,y,w,z)
```
Ответ: zyxw
##
20  
№64887  
<img width="730" height="193" alt="image" src="https://github.com/user-attachments/assets/aeeb8460-bb2e-41c7-8e26-2f0dcb8094a2" />  
```
print('x y w z')
for x in range (2):
    for y in range (2):
        for w in range (2):
            for z in range (2):
                if ((x == y) <= ((not z) or w)) == (not((w <= x) or (y <= z))):
                    print(x,y,w,z)
```
Ответ: wzyx
##
21  
№72587  
<img width="748" height="204" alt="image" src="https://github.com/user-attachments/assets/2e34f3dc-bd84-4e0d-87da-dc04d1445110" />  
```
print('x y w z')
for x in range (2):
    for y in range (2):
        for w in range (2):
            for z in range (2):
                if not((x <= (z <= w)) and (z <= (y == (not w)))):
                    print(x,y,w,z)
```
Ответ: zxwy
##
# ТИП - 8
##
1  
№3697   
<img width="845" height="158" alt="image" src="https://github.com/user-attachments/assets/964bc2b8-3821-43de-8d4a-c003cf307784" />
```
from itertools import *
a=0
for i in product('ВИНТ', repeat=5):
    a+=1
    if a == 1019:
        print(a,''.join(i))
```
Ответ: ТТТНН
##
2  
№78064  
<img width="854" height="187" alt="image" src="https://github.com/user-attachments/assets/8e4505b3-8d18-4303-88a2-6819221f4f68" />
```
from itertools import *
a=0
for i in product(sorted('КРОВАТЬ'), repeat=5):
    b=''.join(i)
    a += 1
    if b.count('Т') <= 1 and b.count('В') == 2 and 'ЬЬ' not in b and a % 2 != 0:
        print(a)
```
Ответ: 16277
##
3  
№55625  
<img width="828" height="51" alt="image" src="https://github.com/user-attachments/assets/ebee4e95-6f2d-4dd5-9739-e07629a187fd" />
```
from itertools import *
a=0
cn=0
for i in permutations('ЯРОСЛАВ', r=5):
    sl=''.join(i)
    if sl.count('Я') + sl.count('О') + sl.count('А') < sl.count('Р') + sl.count('С') + sl.count('Л') + sl.count('В') \
    and 'ЯЯ' not in sl and 'ОО' not in sl and 'АА' not in sl and 'ЯО' not in sl and 'ЯА' not in sl \
    and 'ОЯ' not in sl and 'ОА' not in sl and 'АО' not in sl and 'АЯ' not in sl:
        cn+=1
print(cn)
```
Ответ: 1224
##
4  
№7667  
<img width="841" height="33" alt="image" src="https://github.com/user-attachments/assets/42acd06d-5b29-40c4-a7bc-71b0b05985ad" />
```
from itertools import *
a=0
for i in product('ЕГЭ', repeat=5):
    sl=''.join(i)
    if sl[0] == 'Е' or sl[0] == 'Э':
        a+=1
print(a)
```
Ответ:162
##
5  
№17328  
<img width="827" height="33" alt="image" src="https://github.com/user-attachments/assets/aefd119a-b388-4c3c-b2df-59fe606018fd" />  
```
from itertools import *
a=0
for i in permutations("ГЕРАСИМ", r=7):
    sl = "".join(i)
    sl= sl.replace('Г','1')
    sl= sl.replace('Р','1')
    sl= sl.replace('С','1')
    sl= sl.replace('М','1')
    sl= sl.replace('Е','0')
    sl= sl.replace('А','0')
    sl= sl.replace('И','0')
    if '11' not in sl and '00' not in sl:
        a+=1
print(a)
```
Ответ:144
##
6  
№27539  
<img width="832" height="48" alt="image" src="https://github.com/user-attachments/assets/855c4df7-2a19-4af5-8d11-7e38faf4871e" />  
```
from itertools import *
a=0
for i in product("БОРИС", repeat=6):
    sl = "".join(i)
    if sl.count('Б') == 1 and sl.count('Р') == 1 and sl.count('С') <=1:
        a += 1
print(a)
```
Ответ:1440
##
7  
№18491  
<img width="830" height="30" alt="image" src="https://github.com/user-attachments/assets/58a7bb25-630a-4718-8995-eefee9f8a57e" />
```
from itertools import *
a=0
for i in permutations("ОЛЬГА", r=5):
    sl = "".join(i)
    sl = sl.replace('О', '1')
    sl = sl.replace('А', '1')
    if sl[0] != 'Ь' and '1Ь' not in sl:
        a += 1
print(a)
```
Ответ:48
##
8  
№37143  
<img width="836" height="35" alt="image" src="https://github.com/user-attachments/assets/4bb3956c-a200-4920-bedf-8f4ed3c2edbd" />
```
from itertools import *
a=0
for i in product("ГЕПАРД", repeat=5):
    sl = "".join(i)
    if sl[0] != 'А' and sl[-1] != 'Е' and sl.count('Г') == 1:
        a += 1
print(a)
```
Ответ:2200
##
9  
№59745  
<img width="836" height="179" alt="image" src="https://github.com/user-attachments/assets/243ae4a2-b911-4fb6-a793-c0ebf29400a0" />
```
from itertools import *
a=0
c=0
for i in product(sorted("АЛГОРИТМ"), repeat=5):
    a+=1
    sl = "".join(i)
    if a % 2 != 0 and sl.count('И') >= 2 and sl[0] != 'Г':
        c += 1
print(c)
```
Ответ:2429
##
10  
№10473  
<img width="834" height="51" alt="image" src="https://github.com/user-attachments/assets/507c8f92-744b-4a02-a017-c5fa58e141e3" />  
```
from itertools import *
a=0
for i in product('1234', repeat=5):
    sl= ''.join(i)
    if sl.count('1') == 2:
        a+=1
print(a)
```
Ответ:270
##
11  
№60250  
<img width="835" height="34" alt="image" src="https://github.com/user-attachments/assets/037255b7-2dd4-4a19-aa05-e3e2eef0208d" />  
```
from itertools import *
a=0
for i in permutations('0234567', r=5):
    sl= ''.join(i)
    if sl[0] != '0' :
        sl = sl.replace('2','0')
        sl = sl.replace('4', '0')
        sl = sl.replace('6', '0')
        sl = sl.replace('5', '3')
        sl = sl.replace('7', '3')
        if '00' not in sl and '33' not in sl:
            a+=1
print(a)
```
Ответ:180
##
12  
№64938  

```

```
Ответ:
##
13  
№9796  
<img width="832" height="64" alt="image" src="https://github.com/user-attachments/assets/b8eab671-8d0f-40f5-b8fb-6139de69f5a4" />  
```
from itertools import *
a=0
for i in product('ABCX', repeat=5):
    sl=''.join(i)
    if sl.count('X') == 1:
        a+=1
print(a)
```
Ответ:405
##
14  
№27009  
<img width="836" height="49" alt="image" src="https://github.com/user-attachments/assets/2c082e14-7019-444b-8115-221c62633fa2" />  
```
from itertools import *
a=0
for i in product('НИКОЛАЙ', repeat=4):
    sl= ''.join(i)
    sl = sl.replace('И','1')
    sl = sl.replace('О', '1')
    sl = sl.replace('А', '1')
    if sl[0] != 'Й' and sl.count('1') >= 1:
        a+=1
print(a)
```
Ответ:1866
##
15  
№15822  
<img width="833" height="151" alt="image" src="https://github.com/user-attachments/assets/46a90908-2dc0-4a20-b5e6-0ea2adff898d" />  
```
from itertools import *
a=0
for i in product(sorted('РЕКА'), repeat=4):
    sl = ''.join(i)
    a+=1
    if 'А' not in sl:
        print(a,sl)
```
Ответ:86
##
16  
№28546  
<img width="828" height="40" alt="image" src="https://github.com/user-attachments/assets/fc4b953a-a581-456b-bc92-0854fb1c61ce" />  
```
from itertools import *
c=0
a=0
for i in permutations('НАСТЯ', r=4):
    sl = ''.join(i)
    sl = sl.replace('Н','1')
    sl = sl.replace('С', '1')
    sl = sl.replace('Т', '1')
    sl = sl.replace('А', '0')
    sl = sl.replace('Я', '0')
    if '00' not in sl and '11' not in sl:
        c+=1
print(c)
```
Ответ:24
##
17  
№15795  
<img width="837" height="174" alt="image" src="https://github.com/user-attachments/assets/fbec078e-8ff2-4f08-a5f4-bec602f69664" />    
```
from itertools import *
a=0
for i in product(sorted('ПАРУС'), repeat=4):
    sl = ''.join(i)
    a+=1
    if 'А' not in sl:
        print(a,sl)
```
Ответ:157
##
18  
№3700  
<img width="830" height="152" alt="image" src="https://github.com/user-attachments/assets/d6069086-70f0-4ea2-a613-7c0e130b607d" />    
```
from itertools import *
a=0
for i in product('БКФС', repeat=5):
    sl=''.join(i)
    a+=1
    if a == 486:
        print(a,sl)
```
Ответ:КСФКК
##
19  
№3237  
<img width="746" height="125" alt="image" src="https://github.com/user-attachments/assets/6f77ce6f-6500-4499-821b-31470526c833" />    
```
from itertools import *
a=0
for i in product('AOY', repeat=5):
    sl=''.join(i)
    a+=1
    if a == 170:
        print(a,sl)
```
Ответ:YAAYO
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
<img width="845" height="39" alt="image" src="https://github.com/user-attachments/assets/13c1f250-cd46-4e10-af45-53b5c7f1b562" />    
```
from itertools import *
a=0
for i in permutations('0234567', r=5):
    sl = ''.join(i)
    if i[0] != '0':
        sl = sl.replace('3','1')
        sl = sl.replace('5','1')
        sl = sl.replace('7','1')
        sl = sl.replace('2','0')
        sl = sl.replace('4','0')
        sl = sl.replace('6','0')
        if '00' not in sl and '11' not in sl:
            a+=1
print(a)
```
Ответ: 180
##
