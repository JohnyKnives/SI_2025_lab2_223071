# Втора лабораториска вежба по Софтверско инженерство
# Јован Саздановски, бр.на индекс 223071
Control Flow Graph
![Control Flow Graph drawio](https://github.com/user-attachments/assets/4fbdc080-7bf4-48f6-b4bb-c18afe98b019)
Цикломатска комплексност
Цикломатската комплексност на овој код е 9, истата ја добив преку формулата P+1, каде што P е бројот на предикатни јазли. Во случајов P=8, па цикломатската комплексност изнесува 9. P+1=8+1=9

Тест случаи според every statement

allItems = null Се праќа без аргументи и програмата фрла exception 
allItems = {null,10,0,0}  Се праќаат сите аргументи без Name фрла exception
allItems = {("name",100,0,4),("name",380,7,2)}, cardNumber=null  Се праќаат валидни аргументи за items но cardNumber фрла exception
allItems = VALID, cardNumber = 12343218901234AB  се праќа cardNumber со букви и фрла exception
allItems = VALID, cardNumber = VALID  се испраќаат валидни информации и завршува

Со овие 5 тест случаи се поминува низ сите statements во методата.

Тест случаи според критериум Multiple Condition
if (item.getPrice() > 300 || item.getDiscount() > 0 || item.getQuantity() > 10)
![image](https://github.com/user-attachments/assets/b34d3688-68e2-47ee-a5f5-23c8afaa50bb)

FXX - ако барем еден од производите има помала или вредност од 300.

TFX - ако цената е поголема од 300 но попустот е помал од 0

TTF - ако цената е поголема од 300, попустот е поголем од 0 a количината е помала од 10

TTT - ако сите услови се исполнети

Минимален број на тест случаи се 4 бидејќи има 4 логички релевантни комбинации за овој if услов.
