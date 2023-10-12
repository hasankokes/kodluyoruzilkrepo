## ODEV 5

SELECT title, length FROM film
WHERE title LIKE '%n'
ORDER BY length DESC
LIMIT 5;


SELECT title, length FROM film
WHERE title LIKE '%n'
ORDER BY length ASC
OFFSET 5
LIMIT 5;


SELECT * FROM customer
WHERE store_id = 1
ORDER BY last_name DESC
LIMIT 4;

## ODEV 6

SELECT AVG(rental_rate) FROM film;

SELECT COUNT(*) FROM film
WHERE title LIKE 'C%';

SELECT MAX(LENGTH) FROM film
WHERE RENTAL_RATE = 0.99;

SELECT COUNT(DISTINCT replacement_cost) FROM film
WHERE length > 150;


## ODEV 7

SELECT rating, COUNT(*) FROM film
Group BY rating;



SELECT replacement_cost, COUNT(*) FROM film
Group BY replacement_cost
HAVING COUNT(*) > 50;


SELECT store_id, COUNT(*) FROM customer
Group BY store_id;


SELECT country_id, COUNT(city) FROM city
GROUP BY country_id
order by COUNT(city)DESC
LIMIT 1;
