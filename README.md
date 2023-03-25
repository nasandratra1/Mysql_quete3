# Mysql_quete3
mysql> SHOW DATABASES;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| sys                |
| wild               |
| wild_db_quest      |
+--------------------+
6 rows in set (0.14 sec)

mysql> USE wild_db_quest;
Database changed
mysql> SHOW TABLES;
+-------------------------+
| Tables_in_wild_db_quest |
+-------------------------+
| school                  |
| wizard                  |
+-------------------------+
2 rows in set (0.03 sec)

mysql> UPDATE school SET country = 'Sweden' WHERE id = 3;
Query OK, 1 row affected (0.07 sec)
Rows matched: 1  Changed: 1  Warnings: 0

mysql> UPDATE school SET capacity = 700 WHERE id = 7;
Query OK, 1 row affected (0.31 sec)
Rows matched: 1  Changed: 1  Warnings: 0

mysql> DELETE FROM school WHERE name LIKE '%Magic%;
    
mysql> DELETE FROM school WHERE name LIKE '%Magic%;
  
    

mysql> DELETE FROM school WHERE name LIKE '%Magic%';
Query OK, 3 rows affected (0.06 sec)

mysql> SELECT * FROM school;
+----+----------------------------------------------+----------+----------------+
| id | name                                         | capacity | country        |
+----+----------------------------------------------+----------+----------------+
|  2 | Castelobruxo                                 |      380 | Brazil         |
|  3 | Durmstrang Institute                         |      570 | Sweden         |
|  4 | Hogwarts School of Witchcraft and Wizardry   |      450 | United Kingdom |
|  5 | Ilvermorny School of Witchcraft and Wizardry |      300 | USA            |
|  6 | Koldovstoretz                                |      300 | Russia         |
+----+----------------------------------------------+----------+----------------+
5 rows in set (0.00 sec)
