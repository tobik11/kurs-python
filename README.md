# kurs-python
kurs podstaw języka python
![python logo](https://www.python.org/static/community_logos/python-logo-inkscape.svg)

## Programy do zainstalowania:

1. visual studio code (instalacji interpretera dokonuje się z programu)
- VS_code [instalacja programu](https://www.youtube.com/watch?v=6-uTHMKaI4M)
2. lub oddzielnie interpreter pythona oraz edytor pycharm
- python 2.7 [instrukcja instalacji](https://www.youtube.com/watch?v=QYUBz4mrnFU)
- pycharm [instrukcja instalacji](https://www.youtube.com/watch?v=QzcaEELafkE)


## materiały pomocnicze do kursu
1. używanie zmiennych
```python
a = 55
b = 67
c = a + b
d = a/b
e = a//b

nick_name = "homerman"
nock_name2 = "hunger"
merged_nick_name = nick_name + nick_name2
```
2. komentarze
```python
# to jest komentarz jednoliniowy
''' to jest komentarz
    wieloliniowy
    bardzo dlugi'''
```
3. input / output (wejście / wyjście)
```python
print("lubie bigos")
my_string = autko
print ("to jest", my_string)

age = input("podaj swoj wiek")
```

4. listy / tuple (tuplety)
- listy
```python
grocery_list = ['jajka', 'pomidory', 'mleko', litry]
grocery_list[3] += 5
grocery_list[0] = 'marchew'
other_events = ['wstac', 'zjesc', 'kodzic']
to_do_list = [grocery_list, other_events]
print(to_do_list[1][2])
other_events.append('spac')
other_events.insert(1, 'umyc żeby')
other_events.remove('zjesc')
other_events.sort()
other_events.reverse()
del other_events[2]
print(len(to_do_list))
```
- tuplety
```python
my_tuple = (1,2,3,4,5,6,7)
my_list = list(my_tuple)
my_tuple = tuple(my_list)
length = len(my_tuple)  
minimal = min(my_tuple)

```
5. Dictionaries (słowniki)
```python
nick_names = {'maly' : 'Dominik Jasimski', 'szybki': 'Pawel Domoracki'}
print(nick_names['szybki'])
del nick_names['szybki']
nick_names['szybki'] = 'Tomasz Staniszewski'
nick_names.get('szybki')
nick_names.values()
nick_names.keys()

```

6. pętle, instrukcje warunkowe
```python
age = input("podaj swoj wiek")
if((age > 20) and (age < 27):       //and,  or,  not
	print('probably student')
for x in range(0:20):
	print(x, ' ', end='')

for food in grocery_list:
	print(food)
    
num_list = [[1,2,3],[10,20,30],[100,200,300]]
for x in range(0:3):
	for y in range(0:3):
		print(num_list[x][y])
        
import random
rand_num = random.randrange(0,100)
while(rand_num != 13):
	print(rand_num)
rand_num = random.randrange(0,100)
	i = 0
while(i < 98) 
i = rand_num = random.randrange(0,100)
		if i = 19:
			break

```

7. funkcje
```python
def my_function(a, b):
	c = a*b
	return c

```

8. wejście / wyjście
```python

```
9. wejście / wyjście
```python

```
10. wejście / wyjście
```python

```
11. wejście / wyjście
```python

```
