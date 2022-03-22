# divine_number
from random import *

print('Добро пожаловать в числовую угадайку')

print('Нужно выбрать предел диапазона "?"')
a = int(input())
print('Угадайте число от 1 до', a)
n = randint(1, a)
def is_valid(x):
    return x.isdigit() and 1 <= int(x) <= a

chislo = input()

int_chislo = int(chislo)
schet = 0
while int_chislo != n:
    int_chislo = int(chislo)
    if is_valid(chislo) == True:
        schet += 1
        print(is_valid(chislo))
        print('Введено допустимое число')
        if int_chislo > n:
            print('Слишком много, попробуйте еще раз')
        elif int_chislo < n:
            print('Слишком мало, попробуйте еще раз')
        else:
            break

    else:
        print(is_valid(chislo))
        print('А может быть все-таки введем целое число от 1 до ', a)
    chislo = input()


print('Вы угадали, поздравляем!')
print('Колличество попыток:', schet)
print('Спасибо, что играли в числовую угадайку. Еще увидимся...')from random import *

print('Добро пожаловать в числовую угадайку')

print('Нужно выбрать предел диапазона "?"')
a = int(input())
print('Угадайте число от 1 до', a)
n = randint(1, a)
def is_valid(x):
    return x.isdigit() and 1 <= int(x) <= a

chislo = input()

int_chislo = int(chislo)
schet = 0
while int_chislo != n:
    int_chislo = int(chislo)
    if is_valid(chislo) == True:
        schet += 1
        print(is_valid(chislo))
        print('Введено допустимое число')
        if int_chislo > n:
            print('Слишком много, попробуйте еще раз')
        elif int_chislo < n:
            print('Слишком мало, попробуйте еще раз')
        else:
            break

    else:
        print(is_valid(chislo))
        print('А может быть все-таки введем целое число от 1 до ', a)
    chislo = input()


print('Вы угадали, поздравляем!')
print('Колличество попыток:', schet)
print('Спасибо, что играли в числовую угадайку. Еще увидимся...')
