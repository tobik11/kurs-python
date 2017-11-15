# kurs-python
kurs podstaw języka python
![python logo](https://www.python.org/static/community_logos/python-logo-inkscape.svg)

## Programy do zainstalowania:

1. visual studio code (instalacji interpretera dokonuje się z programu)
- VS_code [instalacja programu](https://www.youtube.com/watch?v=6-uTHMKaI4M)
2. lub oddzielnie interpreter pythona oraz edytor pycharm
- python 2.7 [instrukcja instalacji](https://www.youtube.com/watch?v=QYUBz4mrnFU)
- pycharm [instrukcja instalacji](https://www.youtube.com/watch?v=QzcaEELafkE)


## Przykłady kodu do kursu
1. Liczby
```python
a = 12
b = 5
c = a + b  
d = a / b  # d = 2

e = 12.0
f = float(5)
g = e / f
h = e // f
```

2. Tekst
```python
a = 'asdf'
b = "Ain't no rest for the wicked"

nick_name = "Mel"
nick_name2 = "Avio"
merged_nick_name = nick_name + nick_name2

multiline_text = '''Trawo, trawo do kolan!
Podnieś mi się do czoła,
Żeby myślom nie było
Ani mnie, ani pola.'''
```

3. Komentarze
```python
# to jest komentarz jednoliniowy
''' to jest komentarz
    wieloliniowy
    bardzo dlugi'''
```

4. Wejście / wyjście
```python
print "lubie bigos" 
my_string = "autko"
print  "to jest", my_string

age = input("podaj swoj wiek")
```

5. Kolekcje
- listy
```python
grocery_list = ['jajka', 'pomidory', 'mleko', litry]
grocery_list[3] += 5
grocery_list[0] = 'marchew'
other_events = ['wstac', 'zjesc', 'kodzic']
to_do_list = [grocery_list, other_events]
print to_do_list[1][2]
other_events.append('spac')
other_events.insert(1, 'umyc żeby')
other_events.remove('zjesc')
other_events.sort()
other_events.reverse()
del other_events[2]
print len(to_do_list)
```
- indeksowanie
```python
numbers = [3, 1, 4, 1, 5]
first = numbers[0]
last = numbers[-1]
some = numbers[1:3]
```
- tuplety - niezmienna kolekcja
```python
my_tuple = (1,2,3,4,5,6,7)
my_list = list(my_tuple)
my_tuple = tuple(my_list)
length = len(my_tuple)  
minimal = min(my_tuple)
# nie da się zrobić!!! my_tuple[3] = 10
```
- słowniki (dictionaries) - kolekcje z kluczem
```python
nick_names = {'maly' : 'Dominik Jasimski', 'szybki': 'Pawel Domoracki'}
print(nick_names['szybki'])
del nick_names['szybki']
nick_names['szybki'] = 'Bill'
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
		elif i%3 = 0
			continue

```

7. funkcje
```python
def add(a, b):
	c = a*b
	return c
	
print("the returned value = ", add(5, 9))



def fun(a, b, c):
    d = (a + b) / c
    e = a + b / c   # kolejnosc dzialan ma znaczenie
    return d, e

val1, val2 = fun(5, 6, 7)
print("d = ", val1, "  e = ", val2)

```

8. Interakcja z użytkownikiem, manipulacje na łańcuchach
```python
import sys
text_typed = sys.stdin.readLine()
long_string = 'witam, nazywam sie kret'
print(long_string[9:12])
print(long_string[-4:])
long_string.capitalize()
long_string.find('sie')
long_string.replace(‘kret’, ‘krokiet’)	
long_string.strip()	
long_string.split()
s = 'autostrada'
s.isalpha()	
s.isalnum()	

```
9. Obsługa plików:
```python
my_file = open(”text.txt”, ”wb”)	# ”ab+”  reads and appends a file ”r+” reading and writing
my_file.mode()   .name()
.write(bytes('to jest text zapisywany do pliku\n', ‘UTF-8’))	
.close()	.read()

import os
os.remove(”text.txt”)
```
10. interpolacja stringów
```python
name = 'Grzegorz'
ageG = 23
print('My name is {name}, i am {age}'.format(name=name, age=ageG))
print('Once again: I am {}'.format(name))

print('{:>10}'.format('test'))
'{:10}'.format('test')
'{:^6}'.format('zip')
'{:06.2f}'.format(3.141592653589793)

data = {'first': 'Hodor', 'last': 'Hodor!'}
'{first} {last}'.format(**data)

data = [4, 8, 15, 16, 23, 42]
'{d[4]} {d[5]}'.format(d=data)
```

11. Klasy
```python
class Animal:
	__name = ””
	__height = 0
	__tail = None
	
	Def __init__(self, name, height, tail):
		self.__name = name
		self.height = height
		self.tail = tail
	
	def set_name(self, name):
		self.__name = name

	def get_name(self):
		return self.__name
	
	def toString(self):
		return „{} is {} cm heigh”.format(self.__name, self.__height)

cat = Animal(‘bajcur’, 25, ‘long one’)
print(cat.toString())

```
12. Dziedziczenie
```python
class Dog(Animal):
__owner = ””
def __init__(self, name, height, tail, owner):
	self.__owner = owner
	super(Dog, self).__init__(name, height, tail)
# dodać przykład na overwriting funkcji
def multi_sound(self, how_many = None):
	if how_many is None:
		print(self.get_sound())
	else:
		print(self.get_sound() * how_many)
```

13. tajemnica
```python

```

14. tez
```python

```
