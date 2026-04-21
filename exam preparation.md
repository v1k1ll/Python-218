# ПОДГОТОВКА К ЭКЗАМЕНУ. ЗАДАНИЯ НА ПОДБОР.
## ШПАРГАЛКА В САМОМ НАЧАЛЕ
∧ - and,   
∨ - or,  
≡ - ==,   
¬ - not (букву брать в скобки)  
→ - <=

##
ВСЕ ЗАДАНИЯ РЕШАЮТСЯ НА САЙТЕ "СДАМ ЕГЭ".  
##
1  
№ 28677  
<img width="836" height="215" alt="image" src="https://github.com/user-attachments/assets/33c1ed27-5ef7-4cd1-b811-733df48dedbe" />  

##
2
##
3
##
4  
№ 15618  
<img width="839" height="224" alt="image" src="https://github.com/user-attachments/assets/6cc472d2-c6f7-4790-91af-e25e41159acd" />  
Напишем код для подбора значений
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
