# MySQL
## Примеры SQL запросов
### Создадим таблицу `book`
***Со столбцами:*** </br>
`book_id` - ключевой столбец значение которого будет генерироваться автоматически,</br>
`title` - названиями книг с длиной строки 50 символов,</br>
`author` - авторы с длиной строки 30 символов,</br>
`price` - цена, вещественное число с максимальнйо длинйо числа 8 и 2 символа после запятой
```MySQL
      CREATE TABLE book(
    book_id INT PRIMARY KEY AUTO_INCREMENT,
    title VARCHAR(50),
    author VARCHAR(30),
    price DECIMAL(8, 2),
    amount INT
);
```
