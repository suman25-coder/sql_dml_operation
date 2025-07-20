# SQL Data Manipulation Practice

This repository contains SQL scripts for practicing essential Data Manipulation Language (DML) operations including `INSERT`, `UPDATE`, `DELETE`, and handling `NULL` values. These scripts are designed as part of a SQL Developer Internship task focused on database population and cleaning.

---

## 📂 Contents

- `create_tables.sql` — SQL code to create necessary tables
- `insert_data.sql` — Insert multiple records using different techniques
- `update_data.sql` — Update one or more records using conditions
- `delete_data.sql` — Delete specific or all records
- `null_handling.sql` — Examples of how to handle `NULL` values in queries

---

## 🔧 Technologies

- PostgreSQL
- SQL DML commands

---

## 🧠 Key Concepts Covered

- `INSERT INTO ... VALUES (...)`
- Insert multiple rows in a single query
- `UPDATE ... SET ... WHERE ...`
- `DELETE FROM ... WHERE ...`
- Handling missing or `NULL` values using `IS NULL` and `IS NOT NULL`
- Data cleaning and basic data integrity operations

---

## 📌 Example Tables Used

- `authors(author_id, author_name)`


---

## 🗂️ Sample Query Snippets

--1.Use INSERT INTO for adding rows

insert into authors(author_id, author_name) values 
(2,'suraj'),
(3,'vinit'),
(4,'mohit'),
(5,'sachin'),
(6,'saurav'),
(7,'gaurav'),
(8,'rakesh'),
(9,'raushan'),
(10,'nitin');

select * from authors;

---2.Handle missing values using NULL or default
select *from authors
where authors is null;

---3.Use UPDATE and DELETE with WHERE conditions
update authors
set author_name='rahul'
where author_id=4;

--Delete 
delete from authors
where author_id=4;



