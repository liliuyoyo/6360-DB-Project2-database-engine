
Based on java 1.8

We have our source code in "PeppaPigDataBase" folder.And the main method is located in PeppaPigDataSystem\src\userInterface\DatabaseLaunch.java

For your convenience you can execute the .jar

!!! HOW TO USE .JAR :

1.use Command line, go to target directory;

2.enter "java -jar YellowTeam.jar"

3.then you can do all the tests in command line.


------------------------------------------------------------------------------------------------------
Note:

1. Before running program please delete data folder

2.the rowid is displayed on default but cannot be queried upon
	
  rowid is a reserved word by system and cannot be used in any query

3. ascii can be used to compare with an integer

4. Every text type used in a query must be surrounded by ''
  Ex: 'harry' 

------------------------------------------------------------------------------------------------------

[[[ test queries ]]]

>>>>> show help message <<<<

help;



>>>>> creat table query <<<<<<

create table tb1(p int,age int);

create table tb2(name text,phone_num int,address text);



>>>>> insert into query <<<<<<

insert into table (p,age) tb1 values (1,18);

insert into table (p,age) tb1 values (2,28);

insert into table (name,phone_num,address) tb2 values ('harry',123456789,'magic world on earth');

insert into table (name,phone_num,address) tb2 values ('potter',111111111,'love and be lover');



>>>>> show tables query <<<<

show tables;



>>>>> select query <<<<<<

select * from tb2;

select age from tb1 where age=18;

select age from tb1 where age>1;

select name,phone_num from tb2 where phone_num=111111111;



>>>>> update query <<<<<<

update table tb1 set age=99 where p=1;

select * from tb1;




>>>>> delete query <<<<<<

delete from tb1 where age=28;

select * from tb1;



>>>> logical condition <<<<

select * from tb1 where not age=18;

Select * from tb2 where name='harry' and phone_num=123456789;

Select * from tb2 where name='harry' or name='potter';



>>>>> drop query <<<<<<

drop table tb1;

Show tables;


>>>> create index <<<<<

create index tb2_name on tb2 (name);



>>>> drop index <<<<<

drop index tb2.tb2_name;



>>>>> exit program <<<<<

exit;

