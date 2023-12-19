````Question 1````

test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
````sql
CREATE TABLE employee(
	id INT,
	name VARCHAR(50),
	birthday DATE,
	email VARCHAR(100)
);


````
````Question 2````

Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

````Question 3````

Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
````sql
UPDATE employee
SET name = 'Cafer'
WHERE birthday = '2018-07-21';


UPDATE employee
SET name = 'Mehmet',
	birthday = '1949-08-09',
	email = 'odenmehmet70@gmail.com'
WHERE id = 12;


UPDATE employee
SET birthday = '1954-01-01',
	name = 'Micky',
	email = 'mick@xmail.com'
WHERE id = 35;


UPDATE employee
SET name = 'Ali',
	email = 'ali@xmail.com'
WHERE id = 17;


UPDATE employee
SET email = 'red@panther.com'
WHERE name = 'Charles';
````
````Question 4````

Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
````sql
DELETE FROM employee
WHERE id = 12;


DELETE FROM employee
WHERE birthday = '2108-07-21';


DELETE FROM employee
WHERE email ='mick@xmail.com';


DELETE FROM employee
WHERE name = 'Mehmet';


DELETE FROM employee
WHERE email ='ali@xmail.com';
````
