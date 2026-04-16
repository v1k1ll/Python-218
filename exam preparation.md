# ПОДГОТОВКА К ЭКЗАМЕНУ. ЗАДАНИЯ НА ПОДБОР.
## ШПАРГАЛКА В САМОМ НАЧАЛЕ
∧ - and,   
∨ - or,  
≡ - ==,   
¬ - not (букву брать в скобки)  
→ - <=

##
ВСЕ ЗАДАНИЯ РЕШАЮТСЯ НА САЙТЕ "СДАМ ЕГЭ".  
№ 15618  
<img width="843" height="231" alt="image" src="https://github.com/user-attachments/assets/a242d36d-76a3-4ae2-b352-3c61ae62248c" />  
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
