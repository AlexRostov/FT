Итоговая проверочная работа
Создать репозиторий на GitHub.
Нарисовать блок-схему алгоритма (можно обойтись блок-схемой основной содержательной части, если вы выделяете её в отдельный метод)
Снабдить репозиторий оформленным текстовым описанием решения (файл README.md)
Написать программу, решающую поставленную задачу
Использовать контроль версий в работе над этим небольшим проектом (не должно быть так что все залито одним коммитом, как минимум этапы 2, 3 и 4 должны быть расположены в разных коммитах)
Задача: Написать программу, которая из имеющегося массива строк формирует массив из строк, длина которых меньше либо равна 3 символа. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.
Пример:
["hello", "2", "world", ":-)"] -> ["2", ":-)"]
["1234", "1567", "-2", "computer science"] -> ["-2"]
["Russia", "Denmark", "Kazan"] -> []

Ссылка на репозиторий на GitHub: https://github.com/AlexRostov/FT.git
Блок-схема алгоритма (основана на псевдокоде): Увы.. что-то пошло не так
Алгоритм решения: создаём вспомогательный массив "res" такой же длины, как и первоначально заданный "array", по умолчанию заполненный нулевыми элементами (в C# для типа данных string таким элементом является null значение) и заполняем элементами длина которых меньше либо равна 3 по условию задачи. Считаем количество не нулевых элементов в полученном вспомогательном массиве. На основании этого числа инициализируем целевой массив длинной равной количеству подсчитанных не нулевых значений во вспомогательном массиве.