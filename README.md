# GD
Групповая динамика 
# Программа для получения номера числа Фибоначчи
## Интерфейс
+ **Поле** для ввода номера 
+ Поле для вывода числа Фибоначчи
+ **Кнопка** "Расчитать"
+ Поле для вывода дополнительной информации
## Функции программы
+ Расчёт числа Фибоначчи по его номеру
## Дополнительная информация
[Подробнее о числе Фибоначчи...](https://ru.wikipedia.org/wiki/Фибоначчи)
## Основной код
```
void prime(int N)
        {
            int n = 1000;
            int k = 0;
            int len = n + 1;
            int[] primes = new int[len];
            var prim = new List<int>();
            
            for (int i = 0; i < len; i++)
                primes[i] = i;

            for (int i = 2; i < len; i++)
            {
                for (int j = i + 1; j < len; j++)
                {
                    if (primes[j] == 0)
                        continue;
                    if (j % i == 0)
                    {
                        primes[j] = 0;
                        continue;
                    }
                }
            }
            for (int i = 0; i < len; i++)
            {
                if (primes[i] != 0 && k<N+1 )
                {
                    k++;
                    textBox2.Text = primes[i].ToString();
                }
            }

        }
        
```
## Экранные формы
### Вариант №1
![image](https://user-images.githubusercontent.com/106920559/172060749-3f3bdd89-47fb-4676-b60c-16d254c80408.png)
### Вариант №2
![image](https://user-images.githubusercontent.com/106920559/172060868-7fef5b28-bfc5-4321-9c0b-4eec4b02de99.png)
### Вариант №3
![image](https://user-images.githubusercontent.com/106920559/172060887-916c904b-830b-4753-8500-394d02b04f75.png)
## Выпуски
### Версия 1.1
+ Добавлены поля ввода и вывода чисел
+ Добавлена кнопка "Рассчитать" 
+ Добавлен алгоритм расчёта числа Фибоначчи 
