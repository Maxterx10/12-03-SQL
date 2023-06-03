# Домашнее задание к занятию "`12.3. SQL. Часть 1.`" - `Белов Максим`


### Задание 1

SELECT DISTINCT district  FROM address a
WHERE district LIKE 'K%a' AND district NOT LIKE '% %';

![alt text](https://github.com/Maxterx10/12-02-DDL/blob/main/12-03-1.png)

---

### Задание 2

SELECT * FROM payment p 
WHERE DATE(payment_date) BETWEEN '2005-06-15' AND '2005-06-18'
AND amount > 10;

![alt text](https://github.com/Maxterx10/12-02-DDL/blob/main/12-03-2.png)

---

### Задание 3

SELECT * FROM rental r ORDER BY rental_date DESC
LIMIT 5;

![alt text](https://github.com/Maxterx10/12-02-DDL/blob/main/12-03-3.png)

---


### Задание 4

SELECT customer_id, REPLACE(LOWER(first_name), 'll', 'pp'), 
       LOWER(last_name), active FROM customer c 
WHERE active = '1' AND (first_name = 'kelly' OR first_name = 'willie');

![alt text](https://github.com/Maxterx10/12-02-DDL/blob/main/12-03-4.png)
