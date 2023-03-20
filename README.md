# SQL_HW_2

## :small_blue_diamond:HW during Vadim Ksendzov course:small_blue_diamond:
```
1. Вывести все поля и все строки.
```
```sql
SELECT * FROM students
```
```
2. Вывести всех студентов в таблице
```
```sql
SELECT * FROM students
```
```
3. Вывести только Id пользователей
```
```sql
SELECT id FROM students
```
```
4. Вывести только имя пользователей
```
```sql
SELECT name FROM students
```
```
5. Вывести только email пользователей
```
```sql
SELECT email FROM students
```
```
6. Вывести имя и email пользователей
```
```sql
SELECT name, email FROM students
```
```
7. Вывести id, имя, email и дату создания пользователей
```
```sql
SELECT id, name, email, created_on FROM students
```
```
8. Вывести пользователей где password 12333
```
```sql
SELECT * FROM students
WHERE password = '12333';
```
```
9. Вывести пользователей которые были созданы 2021-03-26 00:00:00
```
```sql
SELECT * FROM students
WHERE created_on = '2021-03-26 00:00:00';
```
```
10. Вывести пользователей где в имени есть слово Анна
```
```sql
SELECT * FROM students
WHERE name LIKE '%Anna%';
```
```
11. Вывести пользователей где в имени в конце есть 8
```
```sql
SELECT * FROM students
WHERE name LIKE '%8';
```
```
12. Вывести пользователей где в имени есть буква а
```
```sql
SELECT * FROM students
WHERE name LIKE '%a%';
```
 ```
13. Вывести пользователей которые были созданы 2021-07-12 00:00:00
```
```sql
SELECT * FROM students
WHERE created_on = '2021-07-12 00:00:00';
```
```
14. Вывести пользователей которые были созданы 2021-07-12 00:00:00 и имеют пароль 1m313
```
```sql
SELECT * FROM students
WHERE created_on = '2021-07-12 00:00:00' AND password = '1m313'
```
```
15. Вывести пользователей которые были созданы 2021-07-12 00:00:00 и у которых в имени есть слово Andrey
```
```sql
SELECT * FROM students
WHERE created_on = '2021-07-12 00:00:00' AND name LIKE '%Andrey%';
```
```
16. Вывести пользователей которые были созданы 2021-07-12 00:00:00 и у которых в имени есть цифра 8
```
```sql
SELECT * FROM students
WHERE created_on = '2021-07-12 00:00:00' AND name LIKE '%8%';
```
```
17. Вывести пользователя у которых id равен 110
```
```sql
SELECT * FROM students
WHERE id = 110;
```
```
18. Вывести пользователя у которых id равен 153
```
```sql
SELECT * FROM students
WHERE id = 153;
```
```
19. Вывести пользователя у которых id больше 140
```
```sql
SELECT * FROM students
WHERE id > 140;
```
```
20. Вывести пользователя у которых id меньше 130
```
```sql
SELECT * FROM students
WHERE id < 130;
```
```
21. Вывести пользователя у которых id меньше 127 или больше 188
```
```sql
SELECT * FROM students
WHERE id < 127 OR id > 188;
```
```
22. Вывести пользователя у которых id меньше либо равно 137
```
```sql
SELECT * FROM students
WHERE id <= 137;
```
```
23. Вывести пользователя у которых id больше либо равно 137
```
```sql
SELECT * FROM students
WHERE id >= 137;
```
```
24. Вывести пользователя у которых id больше 180 но меньше 190
```
```sql
SELECT * FROM students
WHERE id > 180 and id < 190;
```
```
25. Вывести пользователя у которых id между 180 и 190
```
```sql
SELECT * FROM students
WHERE id >= 180 and id <= 190;
```
```
26. Вывести пользователей где password равен 12333, 1m313, 123313
```
```sql
SELECT * FROM students
WHERE password IN('12333','1m313','123313');
```
```
27. Вывести пользователей где created_on равен 2020-10-03 00:00:00, 2021-05-19 00:00:00, 2021-03-26 00:00:00
```
```sql
SELECT * FROM students
WHERE created_on IN('2020-10-03 00:00:00','2021-05-19 00:00:00','2021-03-26 00:00:00');
```
```
28. Вывести минимальный id
```
```sql
SELECT MIN(id) FROM students;
```
```
29. Вывести максимальный.
```
```sql
SELECT MAX(id) FROM students;
```
```
30. Вывести количество пользователей
```
```sql
SELECT COUNT(id) FROM students;
```
```
31. Вывести id пользователя, имя, дату создания пользователя. Отсортировать по порядку возрастания даты добавления пользователя.
```
```sql
SELECT id, name, created_on FROM students
ORDER BY created_on
```
```
32. Вывести id пользователя, имя, дату создания пользователя. Отсортировать по порядку убывания даты добавления пользователя.
```
```sql
SELECT id, name, created_on FROM students
ORDER BY created_on DESC
```