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

   
   
  
