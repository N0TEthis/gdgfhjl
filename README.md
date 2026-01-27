# gdgfhjl
CREATE TABLE user2 (id int,age int ,name varchar(255) );
insert into user2 values
(1000,16,'miao'),
(1100,17, 'mami'),
(1110,17, 'msms'),
(1111 ,18,'geg')
;
select id , name as "students" , age from user2 ;

CREATE TABLE bb2 (btime timestamp ,ktime timestamp, id int );
insert into bb2 values
( '2023-12-09 9:00:34' , '2023-12-09 18:10:32' ,1000),
( '2023-12-09 8:39:13' , '2023-12-09 15:35:24' ,1100),
( '2023-12-09 10:01:56' , '2023-12-09 15:30:17' ,1110),
( '2023-12-09 7:10:14' , '2023-12-09 16:07:02' , 1111)
;
select btime , ktime as "ktime" , id from bb2 ;

SELECT *             
  FROM user2 as A1
  JOIN bb2  as B1
    ON B1.id = A1.id
   
  








CREATE TABLE marks (name varchar(255) );
insert into marks values
('ford'),
( 'audi')
;
select  name as "marks" from marks ;

CREATE TABLE colors (name varchar(255) );
insert into colors values
( 'red'),
( 'blue'),
( 'green')
;
select  name as "colors" from colors ;


SELECT *             
  FROM marks , colors where mark = 'ford' 
  












CREATE TABLE user2 (id int,age int ,name varchar(255) );
insert into user2 values
(1000,16,'miao'),
(1100,17, 'mami'),
(1110,17, 'msms'),
(1111 ,18,'geg')
;
select id , name as "students" , age from user2 ;

CREATE TABLE bb2 (btime timestamp ,ktime timestamp, id int );
insert into bb2 values
( '2023-12-09 9:00:34' , '2023-12-09 18:10:32' ,1000),
( '2023-12-09 8:39:13' , '2023-12-09 15:35:24' ,1100),
( '2023-12-09 10:01:56' , '2023-12-09 15:30:17' ,1110),
( '2023-12-09 7:10:14' , '2023-12-09 16:07:02' , 1111),
( '2023-12-09 11:23:43' , '2023-12-09 18:30:27' ,1101),
( '2023-12-09 12:41:09' , '2023-12-09 12:42:17' ,1011)
;
select btime , ktime as "ktime" , id from bb2 ;

SELECT *             
  FROM user2 as A1
  right JOIN bb2  as B1
    ON B1.id = A1.id








   CREATE TABLE user2 (name varchar(255) , book varchar(255) );
insert into user2 values
('miao','mim'),
('mami','mim')
;


CREATE TABLE bb2 (name varchar(255), book varchar(255));
insert into bb2 values
( 'oppo' , 'mem'),
( 'geg' , 'mem')
;
 select count(*) from (
SELECT name ,book FROM user2 union
SELECT name ,book FROM user2 union 
SELECT  name, book FROM bb2 );
select count(*) from (
SELECT name ,book FROM user2 union all
SELECT name ,book FROM user2 union all
SELECT  name, book FROM bb2 );

   
   
  





CREATE TABLE user2 (name varchar(255) , age int );
insert into user2 values
('miao', 18),
('mami',19),
('msms',21)
;
select name , age from user2 ;

CREATE TABLE bb2 (name varchar(255), ves int , day0 int  );
insert into bb2 values
('miao', 50 , 23),
('mami',100 , 82),
('msms',10 , 120)
;
select name , ves , day0  from bb2 ;

SELECT *             
  FROM user2 as A1
  left JOIN bb2  as B1
    ON B1.name = A1.name
    order by A1.name desc limit 1;
    
    select avg(ves) from bb2
    group by bb2.name







   CREATE TABLE user2 (dep int , num int , tax int );
insert into user2 values
(1 , 101 , 3),
(2 , 102  ,5),
(1 , 101 , 7),
(2 , 103  ,8),
(3 , 104 , 9),
(1 , 104  ,10)
;
select dep , num , tax from user2 ;

    
    select user2.dep , user2.num , sum(tax) from user2
    group by user2.dep,user2.num
   having user2.dep = 1 and user2.num = 101






   ДОДЕЛАТЬ БЫСТРОГ СЕЙЧАС ЖЕ

   CREATE TABLE pacient (id SERIAL PRIMARY KEY, name varchar(255), pol varchar(255) , dr varchar(255) , adres varchar(255));
insert into pacient (name , pol,dr, adres) values
('miao' , 'female' , '2001-12-12' , 'улицадом'),
('mimi' , 'male' , '2005-14-02' , 'улицадом'),
('geg' , 'mele' , '1900-01-01' , 'подвал')
;
select name , pol , dr , adres from pacient;

CREATE TABLE osmotr (name varchar(255),namev varchar(255) ,data varchar(255) ,osmotr varchar(255) , simptom varchar(255) , diagnoz varchar(255) , predpis varchar(255),id_pacient int);

insert into osmotr (name ,namev ,data  ,osmotr , simptom  , diagnoz  , predpis ) values
('miao' , 'mm' ,'2023-12-09' , 'эндкрнлг' ,  'жирни' , 'худей' , 'miao'),
( 'mimi','mr' ,'2023-12-09' , 'эндкрнлг' ,'худой' , 'жирней' , 'miao'),
('geg' ,'mn' ,'2023-12-09' , 'эндкрнлг' , 'ворчит'  , 'geg' , 'miao')
;
select data ,namev, osmotr , simptom , diagnoz , predpis from bb2;

CREATE TABLE b2 (name varchar(255),namev varchar(255),namel varchar(255) ,sp varchar(255) ,slovop varchar(255) , pobochki varchar(255));
insert into b2 values
('miao' , 'mm' ,'бананы' , 'ящикВДвень' ,  'вовово'  , 'переедание'),
( 'mimi','mr' ,'вода' , 'бочкаВдень' ,'вовово'  , 'недоедание'),
('geg' ,'mn' ,'успокоительные' , 'пачкаВдень' , 'вовово'  , 'сонливость')
;



SELECT *            
FROM user2 as A1
INNER JOIN  bb2 as B1 ON A1.name = B1.name 
INNER JOIN b2 as C1 ON B1.name = C1.name;


     
