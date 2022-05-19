# MySQL
## Примеры SQL запросов
### Создадим таблицу `book`
***Со столбцами:***
`book_id` - ключевой столбец значение которого будет генерироваться автоматически,
`title` - названиями книг с длиной строки 50 символов,
`author` - авторы с длиной строки 30 символов,
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
