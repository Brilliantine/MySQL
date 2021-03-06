# MySQL. Примеры запросов
## Оглавление
- [Таблица.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#таблица)
    - [Создание таблицы.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#создание-таблицы)
    - [Вставка записи в таблицу.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#вставка-записи-в-таблицу)
- [Выборка данных.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-данных)
    - [Выборка всех данных из таблицы.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-всех-данных-из-таблицы)
    - [Выборка отдельных столбцов.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-отдельных-столбцов)
    - [Выборка новых столбцов и присвоение им новых имен.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-новых-столбцов-и-присвоение-им-новых-имен)
    - [Выборка данных с созданием вычисляемого столбца.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-данных-с-созданием-вычисляемого-столбца)
    - [Выборка данных, вычисляемые столбцы, логические функции.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-данных-вычисляемые-столбцы-логические-функции)
    - [Выборка данных по условию.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-данных-по-условию)
    - [Выборка данных, логические операции.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-данных-логические-операции)
    - [Выборка данных, операторы BETWEEN, IN.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-данных-операторы-between-in)
    - [Выборка данных с сортировкой (ORDER BY).](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-данных-с-сортировкой-order-by)
    - [Выборка данных, оператор LIKE.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-данных-оператор-like)
- [Запросы, групповые операции.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#запросы-групповые-операции)
    - [Выбор уникальных элементов столбца.](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выбор-уникальных-элементов-столбца)
    - [Выборка данных, групповые функции SUM и COUNT](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-данных-групповые-функции-sum-и-count)
    - [Выборка данных, групповые функции MIN, MAX и AVG](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-данных-групповые-функции-min-max-и-avg)
    - [Выборка данных c вычислением, групповые функции](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-данных-c-вычислением-групповые-функции)
    - [Вычисления по таблице целиком](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#вычисления-по-таблице-целиком)
    - [Выборка данных по условию, групповые функции, WHERE и HAVING](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#выборка-данных-по-условию-групповые-функции-where-и-having)
 - [Вложенные запросы](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#вложенные-запросы)
    - [Вложенный запрос, возвращающий одно значение](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#вложенный-запрос-возвращающий-одно-значение)
    - [Использование вложенного запроса в выражении](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#использование-вложенного-запроса-в-выражении)
    - [Вложенный запрос, операторы ANY и ALL](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#вложенный-запрос-операторы-any-и-all)
    - [Вложенный запрос после SELECT](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#вложенный-запрос-после-select)
 - [Запросы корректировки данных](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#запросы-корректировки-данных)
    - [Добавление записей из другой таблицы](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#добавление-записей-из-другой-таблицы)
    - [Добавление записей, вложенные запросы](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#добавление-записей-вложенные-запросы)
    - [Запросы на обновление](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#запросы-на-обновление)
    - [Запросы на обновление нескольких столбцов](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#запросы-на-обновление-нескольких-столбцов)
    - [Запросы на обновление нескольких таблиц](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#запросы-на-обновление-нескольких-таблиц)
    - [Запросы на удаление](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#запросы-на-удаление)
    - [Запросы на создание таблицы](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#запросы-на-создание-таблицы)
 - [Связи между таблицами](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#связи-между-таблицами)
    - [Создание таблицы с внешними ключами](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#создание-таблицы-с-внешними-ключами)
    - [Действия при удалении записи главной таблицы](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#действия-при-удалении-записи-главной-таблицы)
 - [Запросы на выборку, соединение таблиц](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#запросы-на-выборку-соединение-таблиц)
    - [Соединение INNER JOIN](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#соединение-inner-join)
    - [Внешнее соединение LEFT и RIGHT OUTER JOIN](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#внешнее-соединение-left-и-right-outer-join)
    - [Перекрестное соединение CROSS JOIN](https://github.com/Brilliantine/MySQL/blob/main/SQL.md#перекрестное-соединение-cross-join)

    

## Таблица
### Создание таблицы
***Создадим таблицу `book`***</br>
***Со столбцами:*** </br>
`book_id` - ключевой столбец с автоматической генерацией значения,</br>
`title` - названиями книг с длиной строки 50 символов,</br>
`author` - авторы с длиной строки 30 символов,</br>
`price` - цена, вещественное число с максимально длинной числа 8 и 2 символа после запятой</br>
`amount` - количество книг на складе, целое число
```MySQL
    CREATE TABLE book(
    book_id INT PRIMARY KEY AUTO_INCREMENT,
    title VARCHAR(50),
    author VARCHAR(30),
    price DECIMAL(8, 2),
    amount INT
);
```
### Вставка записи в таблицу
***Добавим строки в таблицу `book`***</br>
```MySQL
    INSERT INTO book (title, author, price, amount)
    VALUES
      ('Мастер и Маргарита', 'Булгаков М.А.', 670.99, 3),
      ('Белая гвардия', 'Булгаков М.А.', 540.50, 5),
      ('Идиот', 'Достоевский Ф.М.', 460.00, 10),
      ('Братья Карамазовы', 'Достоевский Ф.М.', 799.01, 2),
      ('Стихотворения и поэмы', 'Есенин С.А.', 650.00, 15);
 ```
## Выборка данных
### Выборка всех данных из таблицы
```MySQL
    SELECT * FROM book;
 ```
 ***Результат:***</br>
![2022-05-19_17-11-30](https://user-images.githubusercontent.com/40222971/169314643-8caf59c8-7bd9-43c2-8752-219eea4ee429.png)
### Выборка отдельных столбцов
***Запрос:***
```MySQL
    SELECT author, title, price FROM book;
 ```
 ***Результат:***</br>
 ![2022-05-19_17-15-53](https://user-images.githubusercontent.com/40222971/169315468-ffce4296-bdde-46b3-a063-1a14d725ef3c.png)
 ### Выборка новых столбцов и присвоение им новых имен
 ***Запрос:***
 ```MySQL
    SELECT title AS Название, author AS Автор  FROM book;
 ```
 ***Результат:***</br>
 ![2022-05-19_17-20-10](https://user-images.githubusercontent.com/40222971/169316685-3e311e00-107a-4b0b-9633-29a80a6175b4.png)
### Выборка данных с созданием вычисляемого столбца
 Посчитаем стоимость упаковки для каждой книги. При условии что для упаковки каждой книги требуется один лист бумаги, цена которого 1 рубль 65 копеек. Отдельным столбцом выделим стоимость упаковки.</br>
***Запрос:***
```MySQL
    SELECT title, amount, amount * 1.65 AS pack FROM book;
```
***Результат:***</br>
![2022-05-19_17-25-48](https://user-images.githubusercontent.com/40222971/169318773-c31fcb90-3bf6-4f71-934f-193896d7a642.png)
### Выборка данных, вычисляемые столбцы, логические функции
Поднимим цену книг Булгакова на 10%, а цену книг Есенина - на 5%. Напишем запрос, куда включим автора, название книги и новую цену, последний столбец назавём `new_price`. Значение округлим до двух знаков после запятой.</br>
***Запрос:***
```MySQL
    SELECT author, title,
    ROUND (IF(author =  'Булгаков М.А.',price + price*0.1,IF(author = 'Есенин С.А.', price + price * 0.05, price)),2)
    AS new_price FROM book;
```
***Результат:***</br>
![2022-05-19_17-31-34](https://user-images.githubusercontent.com/40222971/169320944-5490be89-5dbe-4600-b816-ba2e5ef5b739.png)
### Выборка данных по условию
Выведем автора, название  и цены тех книг, количество которых меньше 10.</br>
***Запрос:***
```MySQL
    SELECT author, title, price FROM book WHERE amount < 10;
```
***Результат:***</br>
![2022-05-19_17-36-09](https://user-images.githubusercontent.com/40222971/169322457-8288fb95-540c-4398-a544-b23c145a72f2.png)
### Выборка данных, логические операции
Выведем название, автора,  цену  и количество всех книг, цена которых меньше 500 или больше 600, а стоимость всех экземпляров этих книг больше или равна 5000.</br>
***Запрос:***
```MySQL
    SELECT title, author, price, amount
    FROM book
    WHERE (price < 500 OR price > 600) AND price*amount >= 5000;
```
***Результат:***</br>
![2022-05-19_18-06-17](https://user-images.githubusercontent.com/40222971/169329090-41cbbf0a-b343-4669-b94e-0b07840e3fc2.png)
### Выборка данных, операторы BETWEEN, IN
Выведем название и авторов тех книг, цены которых принадлежат интервалу от 540.50 до 800 (включая границы),  а количество или 2, или 3, или 5, или 7.</br>
***Запрос:***
```MySQL
    SELECT title, author
    FROM book
    WHERE (price BETWEEN 540.50 AND 800) AND amount IN (2, 3, 5, 7);
```
***Результат:***</br>
![2022-05-19_18-12-42](https://user-images.githubusercontent.com/40222971/169331153-6e2db37d-6d95-432a-8eed-bf8dba0aa4f4.png)
### Выборка данных с сортировкой (ORDER BY)
Выведем  автора и название  книг, количество которых принадлежит интервалу от 2 до 14 (включая границы). Информацию  отсортируем сначала по авторам (в обратном алфавитном порядке), а затем по названиям книг (по алфавиту).</br>
***Запрос:***
```MySQL
    SELECT author, title
    FROM book
    WHERE amount
    BETWEEN 2 AND 14
    ORDER BY 1 DESC,2;
```
***Результат:***</br>
![2022-05-19_18-18-52](https://user-images.githubusercontent.com/40222971/169333382-b89226ab-bc6c-4d3a-907b-6e787ddee305.png)
### Выборка данных, оператор LIKE
Выведем название и автора тех книг, название которых состоит из двух и более слов, а инициалы автора содержат букву «С». Будем считать, что в названии слова отделяются друг от друга пробелами и не содержат знаков препинания, между фамилией автора и инициалами обязателен пробел, инициалы записываются без пробела в формате: буква, точка, буква, точка. Информацию отсортируем по названию книги в алфавитном порядке.</br>
***Запрос:***
```MySQL
    SELECT title, author
    FROM book
    WHERE title LIKE "%_% %_%" AND author LIKE "%С.%"
    ORDER BY title;
```
***Результат:***</br>
![2022-05-19_20-04-43](https://user-images.githubusercontent.com/40222971/169357530-1fbea54e-2846-4dce-a780-00692f4c5fab.png)
## Запросы, групповые операции
### Выбор уникальных элементов столбца
Выбререм различных авторов, книги которых хранятся в таблице `book`с помощью оператора `DISTINCT`.</br>
***Запрос:***
```MySQL
    SELECT DISTINCT author
    FROM book;
```
***Результат:***</br>
![2022-05-19_20-11-44](https://user-images.githubusercontent.com/40222971/169358590-c732f3c2-d479-44b2-b811-100126eb581c.png)
ОтобTHTV уникальные элементы столбца `amount` таблицы `book` при помощи `GROUP BY`.</br>
***Запрос:***
```MySQL
    SELECT amount
    FROM book
    GROUP BY amount;
```
***Результат:***</br>
![2022-05-19_20-16-11](https://user-images.githubusercontent.com/40222971/169359279-f90abb7f-da1f-457f-9450-c133aeb7c685.png)
### Выборка данных, групповые функции SUM и COUNT
Посчитаем, количество различных книг и количество экземпляров книг каждого автора , хранящихся на складе.  Столбцы назвавём `Автор`, `Различных_книг` и `Количество_экземпляров` соответственно.</br>
***Запрос:***
```MySQL
    SELECT author AS Автор,
           count(amount) AS Различных_книг,
           sum(amount) AS Количество_экземпляров
    FROM book
    GROUP BY author;
```
***Результат:***</br>
![2022-05-19_20-23-36](https://user-images.githubusercontent.com/40222971/169360558-44f55d1e-731a-4a8f-ad40-b3ca359cfdda.png)
### Выборка данных, групповые функции MIN, MAX и AVG
Выведем фамилию и инициалы автора, минимальную, максимальную и среднюю цену книг каждого автора . Вычисляемые столбцы назавём `Минимальная_цена`, `Максимальная_цена` и `Средняя_цена` соответственно.</br>
***Запрос:***
```MySQL
    SELECT author,
           MIN(price) AS Минимальная_цена,
           MAX(price) AS Максимальная_цена,
           AVG(price) AS Средняя_цена
    FROM book
    GROUP BY author;
```
***Результат:***</br>
![2022-05-19_20-37-29](https://user-images.githubusercontent.com/40222971/169363000-a10b5bde-ed79-40e4-bca0-a47d6f606349.png)
### Выборка данных c вычислением, групповые функции
Для каждого автора вычислим суммарную стоимость книг, а также вычислим налог на добавленную стоимость  для полученных сумм, который включен в стоимость и составляет k = 18%,  а также стоимость книг без него. Значения округлим до двух знаков после запятой.</br>
***Запрос:***
```MySQL
    SELECT author,
           SUM(ROUND(price*amount,2)) AS Стоимость,
           SUM(ROUND((price*amount*0.18)/(1+0.18),2)) AS НДС,
           SUM(ROUND((price*amount)/(1+0.18),2)) AS Стоимость_без_НДС
           FROM book
           GROUP BY author;
```
***Результат:***</br>
![2022-05-19_20-43-37](https://user-images.githubusercontent.com/40222971/169364079-a68150aa-1dab-4ff5-8261-365220c2454f.png)
### Вычисления по таблице целиком
Выведем  цену самой дешевой книги, цену самой дорогой и среднюю цену уникальных книг на складе. Среднюю цену округлим до двух знаков после запятой.</br>
***Запрос:***
```MySQL
    SELECT MIN(price) AS Минимальная_цена,
           MAX(price) AS Максимальная_цена,
           ROUND(AVG(price),2) AS Средняя_цена
           FROM book;
```
***Результат:***</br>
![2022-05-19_20-46-44](https://user-images.githubusercontent.com/40222971/169364612-78f601f0-bfb0-43a1-b7ce-29a59b787260.png)
### Выборка данных по условию, групповые функции, WHERE и HAVING
Выведем максимальную и минимальную цену книг каждого автора, кроме Есенина, количество экземпляров книг которого больше 10.</br>
***Запрос:***
```MySQL
    SELECT author,
           MIN(price) AS Минимальная_цена,
           MAX(price) AS Максимальная_цена
    FROM book
    WHERE author <> 'Есенин С.А.'
    GROUP BY author
    HAVING SUM(amount) > 10;
```
***Результат:***</br>
![2022-05-19_20-51-37](https://user-images.githubusercontent.com/40222971/169365453-e34fae7d-6425-4025-b2c6-1248bb4266c1.png)

Посчитаем стоимость всех экземпляров каждого автора без учета книг «Идиот» и «Белая гвардия». В результат включим только тех авторов, у которых суммарная стоимость книг (без учета книг «Идиот» и «Белая гвардия») более 5000 руб. Вычисляемый столбец назваём `Стоимость`. Результат отсортируем по убыванию стоимости.</br>
***Запрос:***
```MySQL
    SELECT author,
           ROUND(SUM(price*amount),2) AS Стоимость
    FROM book
    WHERE title NOT IN('Идиот','Белая гвардия')
    GROUP BY author
    HAVING ROUND(SUM(price*amount),2)>5000
    ORDER BY Стоимость DESC;
```
***Результат:***</br>
![2022-05-19_20-57-27](https://user-images.githubusercontent.com/40222971/169366839-dd469770-b37a-41c2-9a97-20d7a4beb673.png)
## Вложенные запросы
### Вложенный запрос, возвращающий одно значение
Выведем информацию (автора, название и цену) о  книгах, цены которых меньше или равны средней цене книг на складе. Информацию выведем в отсортированном по убыванию цены виде. Среднее вычислим как среднее по цене книги.</br>
***Запрос:***
```MySQL
    SELECT author, title, price FROM book
    WHERE price<=(
        SELECT AVG(price)
        FROM book)
    ORDER BY price DESC;
```
***Результат:***</br>
![2022-05-19_21-00-47](https://user-images.githubusercontent.com/40222971/169368404-64f5853c-0692-474b-b610-cfe7bddb3fa5.png)
### Использование вложенного запроса в выражении
Выведем информацию (автора, название и цену) о тех книгах, цены которых превышают минимальную цену книги на складе не более чем на 150 рублей в отсортированном по возрастанию цены виде.</br>
***Запрос:***
```MySQL
    SELECT author, title, price
    FROM book
    WHERE price <= (SELECT MIN(price) FROM book) + 150
    ORDER BY price ASC;
```
***Результат:***</br>
![2022-05-19_21-06-43](https://user-images.githubusercontent.com/40222971/169369951-fde44d38-3689-467e-81d9-46fa78abc643.png)
#### Вложенный запрос, оператор IN
Выведем информацию (автора, книгу и количество) о тех книгах, количество экземпляров которых в таблице `book` не дублируется.</br>
***Запрос:***
```MySQL
    SELECT author, title, amount FROM book
    WHERE amount IN (
           SELECT amount FROM book
           GROUP BY amount
   HAVING COUNT(amount) = 1);
```
***Результат:***</br>
![2022-05-19_21-09-51](https://user-images.githubusercontent.com/40222971/169371215-5438e5f1-6098-45d3-9d37-6fa2460e0b03.png)
### Вложенный запрос, операторы ANY и ALL
Выведем информацию о книгах(автор, название, цена), цена которых меньше самой большой из минимальных цен, вычисленных для каждого автора.</br>
***Запрос***
```MySQL
    SELECT author, title, price FROM book
    WHERE price < ANY (
            SELECT AVG(price) FROM book
            GROUP BY author);
```
***Результат:***</br>
![2022-05-19_22-45-25](https://user-images.githubusercontent.com/40222971/169389975-74cf115b-0733-4620-abff-e092a7727c8c.png)

Выведем информацию о тех книгах, количество которых меньше самого маленького среднего количества книг каждого автора.</br>
***Запрос:***
```MySQL
    SELECT title, author, amount, price
    FROM book
    WHERE amount < ALL (
        SELECT AVG(amount) 
        FROM book 
        GROUP BY author 
      );
```
***Результат:***</br>
![2022-05-19_22-42-10](https://user-images.githubusercontent.com/40222971/169389450-d7f0a54b-a698-4350-897d-c1686e86449d.png)

### Вложенный запрос после SELECT
Посчитаем сколько и каких экземпляров книг нужно заказать поставщикам, чтобы на складе стало одинаковое количество экземпляров каждой книги, равное значению самого большего количества экземпляров одной книги на складе. Выведем название книги, ее автора, текущее количество экземпляров на складе и количество заказываемых экземпляров книг. Последнему столбцу присвоии имя `Заказ`. В результат не включим книги, которые заказывать не нужно.</br>
***Запрос:***
```MySQL
    SELECT title, author, amount,
           (SELECT MAX(amount) FROM book) - amount AS Заказ
    FROM book
    WHERE amount < (SELECT MAX(amount) FROM book);
```
***Результат:***</br>
![2022-05-19_22-51-55](https://user-images.githubusercontent.com/40222971/169392131-46e1e034-6a0f-47ec-89b4-8d9b017e58ad.png)
## Запросы корректировки данных
Создадим новую таблицу `supply`.</br>
***Запрос:***
```MySQL
    CREATE TABLE supply (
    supply_id INT PRIMARY KEY AUTO_INCREMENT,
    title VARCHAR(50),
    author VARCHAR(30),
    price DECIMAL(8,2),
    amount INT
    );
```
Добавим записи в нашу таблицу.</br>
***Запрос:***
```MySQL
INSERT INTO supply (title, author, price, amount)
VALUES
        ('Лирика', 'Пастернак Б.Л.', 518.99, 2),
        ('Черный человек', 'Есенин С.А.', 570.20, 6),
        ('Белая гвардия','Булгаков М.А.', 540.50, 7),
        ('Идиот', 'Достоевский Ф.М.', 360.80, 3);
```
### Добавление записей из другой таблицы
Добавим из таблицы `supply` в таблицу `book`, все книги, кроме книг, написанных Булгаковым М.А. и Достоевским Ф.М.</br>
***Запрос:***
```MySQL
INSERT INTO book (title, author, price, amount)
SELECT title, author, price, amount
FROM supply
WHERE author NOT IN ('Достоевский Ф.М.','Булгаков М.А.');
SELECT * FROM book;
```
***Результат:***</br>
![2022-05-20_11-03-27](https://user-images.githubusercontent.com/40222971/169482995-8c112301-9a43-4cb7-95a1-41997365986e.png)
### Добавление записей, вложенные запросы
Занесем из таблицы `supply` в таблицу `book` только те книги, авторов которых нет в  `book`.</br>
***Запрос:***
```MySQL
INSERT INTO book (title, author, price, amount)
SELECT title, author, price, amount
FROM supply
WHERE author NOT IN(
    SELECT author FROM book);
SELECT * FROM book;
```
***Результат:***</br>
![2022-05-20_11-09-06](https://user-images.githubusercontent.com/40222971/169484000-5c5506f9-04b0-4f6f-a74a-64ad2e1b980d.png)
### Запросы на обновление
Уменьшим на 10% цену тех книг в таблице `book`, количество которых принадлежит интервалу от 5 до 10, включая границы.</br>
***Запрос:***
```MySQL
UPDATE book
SET price = 0.9 * price
WHERE amount BETWEEN 5 AND 10;
SELECT * FROM book;
```
***Результат:***</br>
![2022-05-20_11-26-47](https://user-images.githubusercontent.com/40222971/169487404-c837f3d2-43e0-4863-80c6-0b2d60a564b7.png)
### Запросы на обновление нескольких столбцов
В таблице `book` скорректируем значение для покупателя в столбце `buy` таким образом, чтобы оно не превышало количество экземпляров книг, указанных в столбце `amount`. А цену тех книг, которые покупатель не заказывал, снизим на 10%.</br>
***Запрос:***
```MySQL
UPDATE book
SET price = IF(buy = 0, price*0.9, price),
    buy = IF(buy > amount, amount, buy);
SELECT * FROM book;
```
***Результат:***</br>
![2022-05-20_11-32-15](https://user-images.githubusercontent.com/40222971/169488294-0580bd8d-7e78-40d1-801f-255eb55de1f1.png)
### Запросы на обновление нескольких таблиц
Для тех книг в таблице `book` , которые есть в таблице `supply`, не только увеличим их количество в таблице `book` ( увеличим их количество на значение столбца `amount` таблицы `supply`), но и пересчитаем их цену (для каждой книги найдем сумму цен из таблиц `book` и `supply` и разделим на 2).</br>
***Запрос:***
```MySQL
UPDATE book, supply
SET book.amount = book.amount + supply.amount,
    book.price = (book.price + supply.price)/2
WHERE book.title = supply.title AND book.author = supply.author;
SELECT * FROM book;
```
***Результат:***</br>
![2022-05-20_11-40-23](https://user-images.githubusercontent.com/40222971/169489715-fa4eecf9-238a-4285-8612-f62fe577ead6.png)
### Запросы на удаление
Удалим из таблицы `supply` книги тех авторов, общее количество экземпляров книг которых в таблице `book` превышает 10.</br>
***Запрос:***
```MySQL
DELETE FROM supply
WHERE author IN(
    SELECT author FROM book
    WHERE amount >= 10
    );
SELECT * FROM supply;
```
***Результат:***</br>
![2022-05-20_11-45-32](https://user-images.githubusercontent.com/40222971/169490799-914a5934-e049-4e2c-851a-0673558b6bee.png)
### Запросы на создание таблицы
Создадим таблицу заказов `ordering`, куда включим авторов и названия тех книг, количество экземпляров которых в таблице `book` меньше среднего количества экземпляров книг в таблице `book`. В таблицу включим столбец `amount`, в котором для всех книг укажем одинаковое значение - среднее количество экземпляров книг в таблице `book`.</br>
***Запрос:***
```MySQL
CREATE TABLE ordering AS
SELECT author, title, (SELECT AVG(amount) FROM book) AS amount
FROM book
WHERE amount < (SELECT AVG(amount) FROM book);
SELECT * FROM ordering;
```
***Результат:***</br>
![2022-05-20_12-05-18](https://user-images.githubusercontent.com/40222971/169494841-220b2f10-4d9a-41e2-8cc0-75a056595902.png)
## Связи между таблицами
Создадим таблицу `author`</br>
***Запрос:***
```MySQL
CREATE TABLE author(
    author_id INT PRIMARY KEY AUTO_INCREMENT,
    name_author VARCHAR(50)
);
```
Заполним таблицу `author`</br>
***Запрос:***
```MySQL
INSERT INTO author(name_author)
VALUES
    ('Булгаков М.А.'),
    ('Достоевский Ф.М.'),
    ('Есенин С.А.'),
    ('Пастернак Б.Л.');
```
### Создание таблицы с внешними ключами
Создадим таблицу `book` таким образом, чтобы ее структура соответствовала структуре, показанной на логической схеме ниже (таблица genre уже создана, порядок следования столбцов - как на логической схеме в таблице `book`, `genre_id`  - внешний ключ).</br>
***Логическая схема:***</br>
![2022-05-20_12-49-59](https://user-images.githubusercontent.com/40222971/169502848-37c97287-8511-4cc3-ac5b-c79c8e8d082b.png)

***Запрос:***</br>
```MySQL
CREATE TABLE book (
    book_id INT PRIMARY KEY AUTO_INCREMENT, 
    title VARCHAR(50), 
    author_id INT NOT NULL,
    genre_id INT,
    price DECIMAL(8,2), 
    amount INT, 
    FOREIGN KEY (author_id)  REFERENCES author (author_id),
    FOREIGN KEY (genre_id) REFERENCES genre (genre_id)
);
```
### Действия при удалении записи главной таблицы
Создать таблицу `book` той же структуры, как в примере выше. Будем считать, что при удалении автора из таблицы `author`, должны удаляться все записи о книгах из таблицы `book`, написанные этим автором. А при удалении жанра из таблицы `genre` для соответствующей записи `book` установить значение `Null` в столбце `genre_id`.</br>
***Запрос:***
```MySQL
CREATE TABLE book (
    book_id INT PRIMARY KEY AUTO_INCREMENT, 
    title VARCHAR(50), 
    author_id INT NOT NULL,
    genre_id INT,
    price DECIMAL(8,2), 
    amount INT, 
    FOREIGN KEY (author_id)  REFERENCES author (author_id) ON DELETE CASCADE,
    FOREIGN KEY (genre_id) REFERENCES genre (genre_id) ON DELETE SET NULL
);
```
## Запросы на выборку, соединение таблиц
### Соединение INNER JOIN
Выведем название, жанр и цену тех книг, количество которых больше 8, в отсортированном по убыванию цены виде.</br>
***Логическая схема:***</br>
![2022-05-20_13-08-01](https://user-images.githubusercontent.com/40222971/169506107-052e9098-8e52-4e43-bf19-08099734c361.png)

***Запрос:***
```MySQL
SELECT title, name_genre, price
FROM
    book INNER JOIN genre
    ON genre.genre_id = book.genre_id AND
    amount >= 8
ORDER BY price DESC;
```
***Результат:***</br>
![2022-05-20_13-09-07](https://user-images.githubusercontent.com/40222971/169506320-bb9397ec-5f07-430a-90ee-c405cf98ba49.png)
### Внешнее соединение LEFT и RIGHT OUTER JOIN
Выведем все жанры, которые не представлены в книгах на складе.</br>
***Логическая схема:***</br>
![2022-05-20_13-19-19](https://user-images.githubusercontent.com/40222971/169507863-5737571c-d154-4a08-8383-629d2019ac43.png)

***Запрос:***
```MySQL
SELECT name_genre
FROM genre LEFT JOIN book
     ON genre.genre_id = book.genre_id
     WHERE title is NULL;
```
***Результат:***</br>
![2022-05-20_13-20-38](https://user-images.githubusercontent.com/40222971/169508063-f6a936f6-cab7-4a8e-be22-014d539a38a3.png)
### Перекрестное соединение CROSS JOIN
Есть список городов, хранящийся в таблице `city`:</br>
![2022-05-20_13-43-39](https://user-images.githubusercontent.com/40222971/169511818-0730a10d-d68a-4065-a2e8-f0845e65c21d.png)</br>
Необходимо в каждом городе провести выставку книг каждого автора в течение 2020 года. Дату проведения выставки выберем случайным образом. Создадим запрос, который выведет город, автора и дату проведения выставки. Последний столбец назвем `Дата`. Информацию выведем, отсортировав сначала в алфавитном порядке по названиям городов, а потом по убыванию дат проведения выставок.</br>
***Запрос:***
```MySQL
SELECT name_city, name_author,
       (DATE_ADD('2020-01-01', INTERVAL FLOOR(RAND()*365) DAY)) as Дата
FROM city, author
ORDER BY city.name_city, Дата DESC;
```
***Результат:***</br>
![2022-05-20_13-48-07](https://user-images.githubusercontent.com/40222971/169512516-4185a276-5435-48d4-941c-0666fa16f2e9.png)
