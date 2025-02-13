# Контрольная работа

## Задача
Написать программу, которая из имеющегося массива строк формирует новый массив из строк, длина которых меньше, либо равна 3 символам. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.

## Блок-схема алгоритма
![Блок-схема алгоритма](diagram.jpg)

## План написания кода:
1. Создать массив строк.
2. Создать пустой массив, который будет хранить отфильтрованные строки.
3. Пройти по каждой строке исходного массива.
Если длина текущей строки меньше или равна 3 символам, добавить эту строку в массив результатов.
4. Вывести на экран отфильтрованный массив строк

## Описание кода:
1. Создать массив строк.
2. Создать пустой массив, который будет хранить отфильтрованные строки.
3. Пройти по каждой строке исходного массива.
Если длина текущей строки меньше или равна 3 символам, добавить эту строку в массив результатов.
4. Вывести на экран отфильтрованный массив строк

## Комментарии к коду
1. Функция CreateArray(int n):
   - Эта функция создает массив строк размером n.
   - Она использует цикл for, чтобы считать n строк с консоли и записать их в массив.
   - Функция возвращает созданный массив строк.

2. Функция CreateConversionArray(string[] array):
   - Эта функция принимает массив строк в качестве аргумента.
   - Она подсчитывает количество строк в исходном массиве, длина которых меньше или равна 3 символам, и записывает это значение в переменную count.
   - Затем она создает новый массив convertArray размером count.
   - Далее она проходит по исходному массиву и копирует в convertArray только те строки, которые удовлетворяют условию array[i].Length <= 3.
   - Функция возвращает новый массив convertArray.

3. Основная часть кода:
   - Сначала программа очищает консоль с помощью Console.Clear().
   - Затем она запрашивает у пользователя размер массива n и считывает его с консоли с помощью Convert.ToInt32(Console.ReadLine()).
   - Далее она использует функцию CreateArray(n) для создания исходного массива строк, и функцию CreateConversionArray(CreateArray(n)) для создания нового массива, содержащего только строки длиной 3 символа или меньше.
   - Наконец, программа выводит отфильтрованный массив ConvertArray в консоль с помощью Console.WriteLine("[{0}]", string.Join(", ", ConvertArray)).

Таким образом, программа создает массив строк, запрашивая их у пользователя, а затем создает новый массив, содержащий только те строки, длина которых меньше или равна 3 символам. Этот отфильтрованный массив выводится в консоль.