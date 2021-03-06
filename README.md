# Test cases for testing a medical mask

Основная  функция медицинской маски - защитная. Защита от вирусов, бактерий, и др. взвешенных частиц, способные проникать через дыхательные пути.
Барьерная - защищает от попадания крови, во время хирургических операций, жидкостей.
Удобство. Неменее важная переменная в медицинской маске. Срок годности маски 2-4 часа.

При тестировании медицинских масок, воспользуемся техникой тест дизайна (эквивалентное разделение, попарное тестирование (уникальные значения)).
Дано 900 шт. медицинских масок, из них 300 шт. - имеют размер S, 300 шт. - M, 300 шт. -L.

| S        | M           | L  |
| ------------- |:-------------|:-------------:|
| 1_S      | 301_M | 601_L |
| 10_S      | 310_M      |   610_L |
| 50_S | 350_M      |    350_L |
| 100_S | 400_M      |    700_L |
| 150_S | 450_M      |    750_L |
| 300_S | 600_M      |    900_L |

Тестируемые медицинские маски:
1_S
10_M
50_L
100_S
150_M
300_L

ID
Priority
Test description
Expected result
Result 
Comment


1. Type
2. Title
3. Precondition
4. Steps
5. Postcondition

Passed
Failed

Задание № 1
01.01
Low
1.  Функциональное тестирование.
2.  Цвет маски
3.
4. 1. Сравнить с образцом голубого цвета (#2196F3)  и его градиентами
5.
Медицинская маска голубого цвета 



01.02
Low
1. Функциональное тестирование.
2. Вес маски
3. Наличие электронных/механических весов
4. 1.Маску положить на электронные/механические весы
5.
Вес медицинской маски 100 г.



01.03
Low
1. Функциональное тестирование.
2. Соответсвие размера 
3. Математическая линейка 
4. 1. При помощи математической линейки измерить каждый край медицинской маски
Размер: 23x13см;



01.04
High
1. Тестирование безопасности.
2. Стерильность (герметичность) упаковки
(Контроль стерилизации мед. изделий проводится при помощи: 1. Физический контроль - состоящий в визуальном и инструментальном контроле за всеми параметрами стерилизации. 2. Химический контроль. 3. Биологический контроль непосредственно указывает, произошло уничтожение микроорганизмов в процессе стерилизации или нет, то есть стерилен или нестерилен объект).
3. Стерильная пробирка для взятия мазка (сваб для взятия мазка), чашка Петри (с наличием пит. среды) автоклав, стерильные услови (мед. лаборатория)
4. 1. С одного края вскрыть упаковку медицинской маски
    2. Незамедлительно, при помощи пробирки взять смыв со всей площади медицинской маски
    3. Взятый материал сеем на питательную среду
    4. Чашку Петри отправляем в автоклав при t = 37’C на 72 часа. 
    5. Невооруженным глазом осматриваем чашку Петри
    6. С помощью микроскопа изучаем питательную среду 
Питательная среда чистая. Патогенной микрофоры не наблюдается



01.05
High
1. Функциональное тестирование.
2. Проверка наличия трёх слоев медицинской маски
3. Ножницы или канцелярский нож
4. 1. Вдоль широкого края медицинской маски провести разрез
    2. Насчитать три фильтрационных слоя
5.
Маска имеет  3 слоя



01.06
Medium
1. Функциональное тестирование.
2. Проверка спайки швов медицинской маски
3. 
4. 1. Визуально осмотреть края медицинской маски
5.
Все 4 стороны медицинской маски имеет хорошо спаяный шов



01.07
Medium
1. Функциональное тестирование.
2. Проверка на гибкость носового фиксатора
3. 
4. 1. Максимально согнуть носовой фиксатор
    2. Максимально разогнуть носовой фиксатор
    3. Повторить 1-2 пункты 3 раза
5.
Носовой фиксатор поддатлив  к применяемой к нему силе.
Гибок.



01.08
High
1. Функциональное тестирование.
2. Проверка крепления ушных резинок
3.
4. 1. Взяться левой рукой за левую ушную резинку медицинской маски
    2. Взяться правой рукой за праую ушную резинку медицинской маски
    3. Продолжая держаться за ушные резинки медицинской маски резко направить руки в противоположные стороны друг от друга.
5.                                 
Маска сохранила свою структуру. Ушные резинки располагаются на месте крепения их к основанию маски.



01.09
Medium
1. Тестирование удобства пользования.
2. Ношение маски в течение трёх часов
3. Человек с размером медицинской маски S, M, L
4. 1. Надеть маску
    2. Отрегулировать носовой фиксатор
    3. Не снимать маску 3 часа
5. 
Не тыльной стороне уха не наблюдается покраснения и мазолей. 
Не спинке носа не наблюдается следов от носового фиксатора.



01.10
Medium
1. Конфигурационное тестирование.
2. Ношение медицинской маски со слуховым аппаратом
3. Слуховой аппарат
4. 1. Надеть маску
Медицинская маска не нарушает работу слухового аппарата.



01.11
High
1. Функциональное тестирование.
2. Исследование проницаемости медицинской маски
3. Пулевизатор с водой + красящее вещество (Балон с краской на водной основе)  (имитация слюных выделений и выделений во время чихания)
4. 1. Надеть маску
    2. Направить пулевизатор на лицевую сторону маски с расстояния 2 метра
    3. Взять чистую маску
    4. Направить пулевизатор на лицевую сторону маски с расстояния 1 метра
Внутренняя сторона медицинской маски чистая, сухая, не пропускает красящее вещество



01.12
Medium
1. Стрессовое тестирование.
2. Поверка состояния маски после заморозки 
3. Морозильная камера (t = - 20’C)
4. 1. Оставить медицинскую маску в морозильной камере на 3 часа
    2. Достать медицинскую маску с морозильной камеры
    3. Дать медицинской маске разморозиться
    4. Дать медицинской маске высохнуть
Медицинская маска не потеряла своей структуры. Цельность сохранена. 



01.13
Medium
1. Стрессовое тестирование.
2. Проверить состояние маски при температуре t= +50’C
3. Термостат
4. 1. Положить медицинскую маску в термостат
    2. Установить t – 50’C на 5 минут
    3. Вытащить маску
Медицинская маска не потеряла своей структуры. Цельность сохранена.



01.14
Medium
1. Стрессовое тестирование.
2. Надежность медицинской маски во время ветра
3. Воздушная пушка (Вентилятор)
4. 1. Направить на маску воздушный потом
Медицинская маска не потеряла своей структуры. Цельность сохранена.













ID
Priority
Test description
Expected result
Result 
Comment


1. Type
2. Title
3. Precondition
4. Steps
5. Postcondition

Passed
Failed

Задание № 2
Поиск изображения
01.01
Medium
1. Негативное тестирование.(Функциональное тестирование)
2. Пустой ввод в поле для ввода ключевого слова
3. Запутить приложение для поиска картинок по ключевому слову
4. 1. Поле для ввода ключевого слова оставить пустым
    2. Нажать кнопку ‘Найти’
Кнопка ‘Найти’ - неактивна
(или появляется сообщение с ошибкой неверного ввода)



01.02
Medium
1. Негативное тестирование.(Функциональное тестирование)
2. Ввод клавиши ‘пробел’ в поле для ввода ключевого слова
3. Запутить приложение для поиска картинок по ключевому слову
4. 1. В поле для ввода ключевого слова ввести клавишу ‘Пробел’
    2. Нажать кнопку ‘Найти’
Кнопка ‘Найти’ - неактивна
(или появляется сообщение с ошибкой неверного ввода)



01.03
Medium
1. Негативное тестирование.(Функциональное тестирование)
2. Максимальное допустимое значение символов
3. Запутить приложение для поиска картинок по ключевому слову
4. 1. Ввести в поле слово состоящее из 261 символов
    2. Нажать кнопку ‘Найти’
Кнопка ‘Найти’ - неактивна
(или появляется сообщение с ошибкой неверного ввода)
(Максимальное допустимое значение в Windows – 260 символов, Linux – 255 символов)



01.04
High
1. Негативное тестирование. (Тестирование безопасности)
2. Ввод юникс-команды, фрагменты кода в поле для ввода ключевого слова
3. Запутить приложение для поиска картинок по ключевому слову
4. 1. Ввести юникс-команду или фрагмент кода
    2. Нажать кнопку ‘Найти’
Появляется сообщение с ошибкой неверного ввода



01.05
Medium
1. Негативное тестирование. (Функциональное тестирование)
2. Ввод специальных символов в поле для ввода ключевого слова
3. Запутить приложение для поиска картинок по ключевому слову
4. 1. Ввести © ® ™ и др.
    2. Нажать кнопку ‘Найти’
Появляется сообщение с ошибкой неверного ввода



Загрузка изображения
02.01
High
1. Негативное тестирование. (Тестирование безопасности)
2. Загрузка файлов с не графическим расширением (txt, exe, mp3 и др)
3. Запутить приложение для поиска картинок по ключевому слову
4. 1. Нажать кнопку ‘Обзор’
    2. Выбрать txt файл
Появляется сообщение с ошибкой о неверном формате файла



02.02
Medium
1. Негативное тестирование. (Функциональное тестирование)
2. Некорректно указан путь к файлу
3. Запутить приложение для поиска картинок по ключевому слову
4. 1. В поле для указывания пути к файлу ввести некорректное значение
    2. Указать ключевое слово
    3. Нажать кнопку ‘Загрузить’
Появляется сообщение с ошибкой: Файл не найден



02.03
Medium
1. Негативное тестирование.(Функциональное тестирование)
2. Пустой ввод в поле для ввода ключевика
3. 
4. 1. Нажать кнопку ‘Обзор’
    2. Выбрать файл с графическим расшиирением
    3. Нажать кнопку загрузить
Появляется сообщение с просьбой указать имя для ключевика



02.04
Medium
1. Негативное тестирование.(Функциональное тестирование)
2. Ввод клавиши ‘пробел’ в поле для ввода ключевика
3. 
4. 1. Нажать кнопку ‘Обзор’
    2. Выбрать файл с графическим расшиирением
    3. В поле для ввода ключевика вводим клачишу ‘Пробел’
    4. Нажать кнопку загрузить
Появляется сообщение с просьбой указать имя для ключевика



02.05
Medium
1. Негативное тестирование.(Функциональное тестирование)
2. Максимальное допустимое значение символов в поле для ключевика
3. 
4. 1. Нажать кнопку ‘Обзор’
    2. Выбрать файл с графическим расшиирением
    3. В поле для ввода ключевика вводим слово состоящее из 261 символа
    4. Нажать кнопку загрузить
Появляется сообщение о недопустимом значении
(или появляется сообщение с ошибкой неверного ввода)
(Максимальное допустимое значение в Windows – 260 символов, Linux – 255 символов)



02.06
High
1. Негативное тестирование. (Тестирование безопасности)
2. Ввод юникс-команды, фрагменты кода в поле для ввода ключевого слова
3. 
4. 1. Нажать кнопку ‘Обзор’
    2. Выбрать файл с графическим расшиирением
    3. В поле для ввода ключевика вводим юникс-команду или фрагмент кода
    4. Нажать кнопку загрузить
Появляется сообщение о недопустимом значении



02.07
Medium
1. Негативное тестирование. (Функциональное тестирование)
2. Ввод специальных символов в поле для ввода ключевика
3. 
4. 1. Нажать кнопку ‘Обзор’
    2. Выбрать файл с графическим расшиирением
    3. В поле для ввода ключевика вводим специальные символы © ® ™
    4. Нажать кнопку загрузить
Появляется сообщение с ошибкой неверного ввода



02.08
Medium
1. Негативное тестирование. (Функциональное тестирование)
2. Ввод цифр в поле для ключевика
3. 
4. 1. Нажать кнопку ‘Обзор’
    2. Выбрать файл с графическим расшиирением
    3. В поле для ввода ключевика вводим цифры (от 1 до 9)
    4. Нажать кнопку загрузить
Появляется сообщение с ошибкой неверного ввода


Если программа не подразумевает ввод чисел в поле для ключевика!
02.09
High
1. Негативное тестирование. (Функциональное тестирование)
2. Загрузка изображения без наличия интернет соединения
3. 
4. 1. Нажать кнопку ‘Обзор’
    2. Выбрать файл с графическим расшиирением
    3. В поле для ввода ключевика слово
    4. Нажать кнопку загрузить
Ошибка – отсутсвие интернет соединения



02.10
High
1. Негативное тестирование. (Функциональное тестирование)
2. Прерывание интернет соединения при загрузке изображения
3. 
4. 1. Нажать кнопку ‘Обзор’
    2. Выбрать файл с графическим расшиирением
    3. В поле для ввода ключевика слово
    4. Нажать кнопку загрузить
    5. Прервать интернет соединение
Появляется сообщение о разрыве интернет соединения. Файл не загружен 



02.11
Medium
1. Негативное тестирование. (Функциональное тестирование)
2. Загрузка одинаковых изображений и одинаковым ключевиком
3. 
4. 1. Нажать кнопку ‘Обзор’
    2. Выбрать файл с графическим расширением
    3. В поле для ввода ключевика слово
    4. Нажать кнопку загрузить
    5. Повторить пункт 1-4
При поиске по данному ключевику  загружается одно фото с данным ключевиком






На выполнение тестового задания потребовался один рабочий день. 
Сожности: отсутсвие подробной спецификации, полагалась на опыт тестировщика и творческий подход.


