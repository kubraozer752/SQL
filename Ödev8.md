# Ödev 8
#### 1.Test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
```sql
CREATE TABLE employee (
	id INTEGER,
	name VARCHAR(50),
	birthday DATE,
	email VARCHAR(100)
	);
```
#### 2.Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
#### 3.Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
```sql
UPDATE employee
SET name = 'Mickey Mouse'
WHERE email LIKE 'm%';
```
```sql
UPDATE employee
SET birthday = '2000-01-01'
WHERE name LIKE 'A%';
```
```sql
UPDATE employee
SET id = '55'
WHERE birthday = '1920-05-26';
```
```sql
UPDATE employee
SET email = 'mickey@mouse.com'
WHERE name LIKE 'S%';
```
```sql
UPDATE employee
SET name = 'Rainbow'
WHERE birthday = '2008-09-14';
```
#### 4.Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
```sql
DELETE FROM employee
WHERE id > 5;
```
```sql
DELETE FROM employee
WHERE name LIKE '%e';
```
```sql
DELETE FROM employee
WHERE birthday = '1909-10-25';
```
```sql
DELETE FROM employee
WHERE email LIKE '%au';
```
```sql
DELETE FROM employee
WHERE id = 5;
```
