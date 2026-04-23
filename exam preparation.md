## ШПАРГАЛКА В САМОМ НАЧАЛЕ
∧ - and,   
∨ - or,  
≡ - ==,   
¬ - not (букву брать в скобки)  
→ - <=

##
ВСЕ ЗАДАНИЯ РЕШАЮТСЯ НА САЙТЕ "СДАМ ЕГЭ".  
##
ТИП - 2
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
№ 15618  
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
Ответ: wzyx
##
