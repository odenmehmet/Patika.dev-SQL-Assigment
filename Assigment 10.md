````Question 1````

city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.
````sql
SELECT city.country_id,country.country_id,city.city, country.country
FROM city LEFT JOIN country ON country.country_id = city.country_id;

````
````Question 2````

customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.
````sql
SELECT customer.first_name, customer.last_name, payment.payment_id
FROM customer 
RIGHT JOIN payment 
ON payment.customer_id = customer.customer_id;
````
````Question 3````

customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.
````sql
SELECT customer.first_name, customer.last_name, rental.rental_id 
FROM customer
FULL JOIN rental
ON customer.customer_id = rental.customer_id;
````
