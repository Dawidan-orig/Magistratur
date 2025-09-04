Контекст таблиц:
CREATE - Создание новой таблицы (отношения)
ALTER - Изменение атрибутов сущностей (Столбцов таблицы)
DROP - Удаление таблицы

Примеры:
```
CREATE TABLE Employees (
EmployeeID INT PRIMARY KEY,    
LastName VARCHAR(50),    
FirstName VARCHAR(50),    
BirthDate DATE,    
Salary DECIMAL(10, 2) );
```

Новый атрибут:
`ALTER TABLE Employees ADD Email VARCHAR(100);`
Изменение атрибута:
`ALTER TABLE Employees ALTER COLUMN Salary DECIMAL(12, 2);`
Удаление атрибута:
`ALTER TABLE Employees DROP COLUMN BirthDate;`

`DROP TABLE {Имя}`

Контекст запиcей:
INSERT - Добавление новой записи
UPDATE - Обновление существующей записи
DELETE - Удаление записи

Примеры:
`INSERT INTO table_name (column1, column2, ...) VALUES (value1, value2, ...);`

`UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition;`

`DELETE FROM table_name WHERE condition;`. Без условия удалит все записи.