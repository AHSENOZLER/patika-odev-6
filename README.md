# patika-odev-6
patika odev 6
--1.film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?
select avg(rental_rate) as "average" from film;

--2.film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?
select count(title) as "toplam" from film
where title ilike('C%');

--3.film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) 
--film kaç dakikadır?
SELECT MAX(length) as 
FROM film 
WHERE rental_rate = 0.99;

--4.film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı 
--replacement_cost değeri vardır?
select count(distinct replacement_cost) from film
where length > 150;
