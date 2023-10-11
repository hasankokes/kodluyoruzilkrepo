## odev2

`SELECT * FROM film
WHERE replacement_cost BETWEEN 12.99 AND 16.99;`

`SELECT first_name, last_name FROM actor
WHERE first_name IN ('Nick','Penelope','Ed');`

`SELECT * FROM film
WHERE rental_rate IN (0.99, 2.99, 4.99) AND replacement_cost IN (12.99, 15.99, 28.99);`


## odev3

`SELECT country FROM country
WHERE country LIKE 'A%a';`

`SELECT country FROM country
WHERE country LIKE '_____%n';`

`SELECT title FROM film
WHERE title ILIKE '%t%t%t%t%';`

`SELECT * FROM film
WHERE title LIKE 'C%'AND length > 90 AND rental_rate IN(2.99);`

## odev4

`SELECT DISTINCT replacement_cost FROM film;`

`SELECT COUNT(DISTINCT replacement_cost) FROM film;`

`SELECT COUNT(title) FROM film
WHERE title LIKE 'T%' AND rating IN ('G');`

`SELECT COUNT(DISTINCT country) FROM country
WHERE country LIKE '_____';`

`SELECT COUNT(DISTINCT city) FROM city
WHERE city ILIKE '%r';`




