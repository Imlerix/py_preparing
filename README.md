
<h1>Python Docs</h1>
<br>
<br>

<h3>Тезисы</h2>
    <ol>
        <li>
            <h4>Переменные </h4>
                 <ul>
                    <li>Никак не объявляются</li>
                    <li>Попытка доступа к не используемой -||- выбросить ошибку</li>
                    <li>a, b = 0, 1 –– множественное присваивание</li>
                 </ul>
        </li>
        <li>
            <h4>Строки </h4>
                 <ul>
                    <li>r 'py /n thon' - необработанные строки</li>
                    <li>''' ''' - многосрочный режим</li>
                    <li>'Py' + 'thon' –– конкатенация</li>
                    <li>3 * 'py' –– повторение</li>
                    <li>Символы строки индексируемы (прямой/обратный порядок)</li>
                    <li>Аналог (в js) slice –– 'Python'[1:3] ==> 'yt'</li>
                    <li>Индекс больший чем длина строки –– ошибка (однако slice работает нормально)</li>
                    <li>'Python'[0] = 'J' –– ошибка</li>
                    <li>'J' + 'Python'[1:] ==> 'Jython' –– правильно</li>
                    <li>len('Python') ==> 6</li>
                 </ul>
        </li>
        <li>
            <h4>Списки </h4>
                 <ul>
                    <li>слайсяться, индексируются, изменяются по индексу</li>
                    <li>array.append(value) аналог push (в js)</li>
                    <li>len(array) длина массива</li>
                    <li>**end** можно использовать, чтобы избежать перехода на новую строку после вывода или завершить вывод другой строкой<pre>```
    while a < 1000 :
      print ( a , end = ',' )
      a , b = b , a + b
==> 0,1,1,2,3,5,8,13,21,34,55,89,144,233,377,610,987,
                     ```</pre></li>
                 </ul>
        </li>
        <li>
            <h4>Циклы и условия </h4>
                 <ul>
                    <li>**if** <pre>```
if x < 0 :
     x = 0
     print ( 'Negative changed to zero' )
elif x == 0 :
     print ( 'Zero' )
                     ```</pre></li>
                     <li>**for** –– аналог for of (в js)<pre>```
words = [ 'cat' , 'window' , 'defenestrate' ]
for item in words :
    print ( item, len( item ))
==> cat 3
==> window 6
==> defenestrate 12
                     ```</pre></li>
                     <li>**range(from, [to, increment])** –– итеративный метод(возвращает список) Если нужно перебрать последовательность чисел. Он генерирует арифметические прогрессии<pre>```
for i in range ( 5 ):
    print ( i )
==> 0
==> 1
==> 2
==> 3
==> 4
//# Диапазоны
range ( 5 , 10 )
==> 5, 6, 7, 8, 9
range ( 0 , 10 , 3 )
==> 0, 3, 6, 9
range ( -10 , -100 , -30 )
==> -10, -40, -70
                     ```</pre></li>
                     <li>range() –– Это объект, который возвращает последовательные элементы желаемой последовательности, когда вы выполняете итерацию, но на самом деле не создает список, тем самым экономя пространство.<pre>```
print ( range ( 10 ))
==> range(0, 10)
//
list ( range ( 4 ))
==> [0, 1, 2, 3]
                     ```</pre></li>
                     <li>**for else**<pre>```
for n in range ( 2 , 10 ):
    for x in range ( 2 , n ):
        if n % x == 0 :
        print ( n , 'equals' , x , '*' , n // x )
        break
    else :
        # loop fell through without finding a factor
        print ( n , 'is a prime number' )
==> 2 is a prime number
==> 3 is a prime number
==> 4 equals 2 * 2
==> 5 is a prime number
==> 6 equals 2 * 3
==> 7 is a prime number
==> 8 equals 2 * 4
==> 9 equals 3 * 3
                     ```</pre></li>
                     <li>**pass** заявление ничего не делает<pre>```
while True :
    pass  # Busy-wait for keyboard interrupt (Ctrl+C)
                     ```</pre></li>
                     <li>есть операторы **continue и break**</li>
                 </ul>
        </li>
        <li>
            <h4>Встроенные функции –– <a>https://clck.ru/Moif6</a></h4>
        </li>
    </ol>