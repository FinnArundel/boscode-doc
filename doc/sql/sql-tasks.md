# SQL tasks

[boscode-learn](https://github.com/Quobject/boscode-learn)

## Table of Content
    
[Installation](#installation)  
[01 - Hello world](#01---hello-world)  

___

## Installation

1. In google chrome open [http://sqlfiddle.com/](http://sqlfiddle.com/).
2. Select `User Options -> Login` and sign in with google +.
3. Select `MySQL 5.6`.



___

## 01 - First table

1. In google chrome open [http://sqlfiddle.com/](http://sqlfiddle.com/).  
2. Click `Clear`.  
3. Inside the left panel (Schema Panel) paste the following sql code:

```sqlfiddle
CREATE TABLE Persons
(
	PersonID int,
	LastName varchar(255),
	FirstName varchar(255),
	Address varchar(255),
	City varchar(255)
);
	

INSERT INTO Persons 
	(PersonID,LastName,FirstName,Address,City) 
VALUES 
	(1,"Merritt","Olivia","Ap #647-3652 Dapibus Avenue","Palanzano"),
	(2,"Workman","Adrienne","P.O. Box 759, 5352 Eros. St.","Kalken"),
	(3,"Dale","Martena","5371 Laoreet St.","Basingstoke"),
	(4,"Paul","Colton","165-2233 Cursus St.","St. John's"),
	(5,"Rice","Oprah","3150 Amet, Road","Frankenthal"),
	(6,"Nash","Hasad","4448 Magna Ave","Orléans"),
	(7,"Ballard","Holly","P.O. Box 793, 460 Justo Av.","Mundare"),
	(8,"Reed","Joan","Ap #742-4973 In Rd.","Móstoles"),
	(9,"Norris","Sean","697-8795 Quam St.","Warrington"),
	(10,"Barrera","Kessie","707-4124 Arcu Av.","Kamarhati")
;
```

4. Click the button `Build Schema`.
5. Inside the right panel paste the following sql code:

```sqlfiddle
SELECT * FROM Persons;
```

6. Click `Run SQL` and observe the output.
7. Inside the right panel modify the sql code:

```sqlfiddle
SELECT FirstName, LastName FROM Persons;
```
8. Click `Run SQL` and observe the output.
9. 4. Learn more about the SQL CREATE TABLE Statement at [w3schools.com](http://www.w3schools.com/sql/sql_create_table.asp).
 

###### The challenge:

1. Write a sql select statement that selects the following three columns: `PersonID`, `LastName`, and `City`.
2. Modify the schema to insert one more record that contains your name and address. In total your insert statement should now contain 11 values.
3. Modify the `CREATE TABLE` statement to add one more column `Postcode`.

___

## 02 - Sequence
