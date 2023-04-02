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
[![cevap 1](https://github.com/OsmanAliWaberi/Fonction-for-select-a-z-/blob/main/1-soru.png)](https://github.com/OsmanAliWaberi/Fonction-for-select-a-z-/blob/main/1-soru.png)


2-
```sql

select * from film where length > 60 and length >75

```
[![cevap 2](https://github.com/OsmanAliWaberi/Fonction-for-select-a-z-/blob/main/2-soru.png)](https://github.com/OsmanAliWaberi/Fonction-for-select-a-z-/blob/main/2-soru.png)

3- 
``` sql

select * from film 
where rental_rate>0.99 and 
( replacement_cost = 12.99 or replacement_cost = 28.99)

```
[![cevap 3](https://github.com/OsmanAliWaberi/Fonction-for-select-a-z-/blob/main/3-soru.png)](https://github.com/OsmanAliWaberi/Fonction-for-select-a-z-/blob/main/3-soru.png)

4- 
```sql

select first_name , last_name from customer where first_name = 'Mary' 

```
[![cevap 4](https://github.com/OsmanAliWaberi/Fonction-for-select-a-z-/blob/main/4-soru.png)](https://github.com/OsmanAliWaberi/Fonction-for-select-a-z-/blob/main/4-soru.png)

5-
```sql

select * from film where length<50 and (rental_rate = 2.99 or rental_rate = 4.99)

```
[![cevap 5](https://github.com/OsmanAliWaberi/Fonction-for-select-a-z-/blob/main/5-soru.png)](https://github.com/OsmanAliWaberi/Fonction-for-select-a-z-/blob/main/5-soru.png)