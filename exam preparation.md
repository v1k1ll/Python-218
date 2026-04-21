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
<img width="844" height="218" alt="image" src="https://github.com/user-attachments/assets/ebb5881d-cd72-48a1-8515-1958edab8fec" />

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
