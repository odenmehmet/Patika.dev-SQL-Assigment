````Question 1:````

film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
````sql
SELECT DISTINCT replacement_cost FROM film ;
````
````Question 2:````

film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
````sql
SELECT COUNT(DISTINCT replacement_cost) FROM film;
````
````Question 3:````

film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
````sql
SELECT COUNT(*) FROM film WHERE title LIKE 'T%' AND rating='G';
````
````Question 4:````

film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
````sql
SELECT COUNT(*) FROM country WHERE country LIKE '_____';
````
````Question 5:````

city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?
````sql
SELECT COUNT(*) FROM city WHERE city ILIKE '%R';
````
