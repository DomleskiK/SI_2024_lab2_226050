Втора лабораториска вежба по Софтверско инженерство
Кристијан Домлески, бр. на индекс 226050


Control Flow Graph
![diagram_softv](https://github.com/DomleskiK/SI_2024_lab2_226050/assets/167032069/ace31e84-5093-4214-bbc3-ed795e40c777)


Цикломатска комплексност
Цикломатска комплексност Цикломатската комплексност на овој код е 10, истата ја добив преку формулата P+1, каде што P е бројот на предикатни јазли. Во случајoв P=9, па цикломатската комплексност изнесува 10.


Тест случаи според критериумот Every statement


allItems = null -> "allItems list can't be null!"

allItems = [("",null,200,0)] -> "No barcode!"

allItems = [("name","kod123",200,0)] -> "Invalid character in item barcode!"

allItems = [("name", "0000",1000,0.1)]; payment = 100 -> false

allItems = [("name", "0000",1000,0)]; payment = 100 -> true


Тест случаи според критериумот Every path



TTT    allItems = [("name","1234",400,0.1)] -> true

TFX    allItems = [("name","1234",400,0.1)] -> false

TTF    allItems = [("name","1234",400,0)] -> false

FXX    allItems = [("name","1234",100,0)] -> false

