# Fonction for select a z
## Odev 1 

**Merhabalar**


Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.

1- film tablosunda bulunan title ve description sütunlarındaki verileri sıralayınız.

2- film tablosunda bulunan tüm sütunlardaki verileri film uzunluğu (length) 60 dan büyük VE 75 ten küçük olma koşullarıyla sıralayınız.

3- film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99 VE replacement_cost 12.99 VEYA 28.99 olma koşullarıyla sıralayınız.
customer tablosunda bulunan first_name sütunundaki değeri 'Mary' olan müşterinin last_name sütunundaki değeri nedir?

4- film tablosundaki uzunluğu(length) 50 ten büyük OLMAYIP aynı zamanda rental_rate değeri 2.99 veya 4.99 OLMAYAN verileri sıralayınız.
Kolay Gelsin.

## Cevaplar


1- 
```sql

select title , description  from film

```



2-
```sql

select * from film where length > 60 and length >75

```


3- 
``` sql

select * from film 
where rental_rate>0.99 and 
( replacement_cost = 12.99 or replacement_cost = 28.99)

```


4- 
```sql

select first_name , last_name from customer where first_name = 'Mary' 

```



5-
```sql

select * from film where length<50 and (rental_rate = 2.99 or rental_rate = 4.99)

```
