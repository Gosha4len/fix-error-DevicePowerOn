#### fix error DevicePowerOn
```
Решение ошибки при запуске VM после её создания VMware Workstation 16:
```
![error](/screenshot/Screenshot_1.png)

```
1) ПКМ по VM - Открыть каталог виртуальной машины :
```
![vm](/screenshot/Screenshot_2.png)

```
Тут нам понадобится выделенный файл с расширением .vmx :
```
![file](/screenshot/Screenshot_3.png)
```
2) Откроем его с помощью любого текстового редактора (в моём примере задействован “Notepad++”) :
```
![notepad](/screenshot/Screenshot_4.png)
```
Тут нам понадобится строчка с кодом vmci0.present = “TRUE” :
```
![vmci0](/screenshot/Screenshot_6.png)
```
3) Меняем значение “TRUE” на “FALSE’ :
```
![vmci0](/screenshot/Screenshot_5.png)
![vmci0](/screenshot/Screenshot_7.png)
```
4) Сохраняем файл :
```
![file](/screenshot/Screenshot_8.png)
```
5) Включаем VM :
```
![start](/screenshot/Screenshot_9.png)
