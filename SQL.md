# MySQL
## Примеры SQL запросов
### Создадим таблицу `book` c ключевым столбцом book_id значение которого будет генерироваться автоматически,
```MySQL
      CREATE TABLE book(
    book_id INT PRIMARY KEY AUTO_INCREMENT,
    title VARCHAR(50),
    author VARCHAR(30),
    price DECIMAL(8, 2),
    amount INT
);
```
