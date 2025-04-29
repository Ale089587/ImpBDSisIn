use Ale089013$default;
Database changed
mysql> 
mysql>  CREATE TABLE DirectorioTelefonico (
    ->      CustomerID INT(6),
    ->     TypePhone VARCHAR(20),
    ->      Number VARCHAR(20)
    ->      );
ERROR 1050 (42S01): Table 'DirectorioTelefonico' already exists
mysql> Show Table DirectorioTelefonico;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syn
tax to use near 'DirectorioTelefonico' at line 1
mysql> SELECT * FROM DirectorioTelefonico;
Empty set (0.01 sec)
mysql> Show Tables;
+-----------------------------+
| Tables_in_Ale089013$default |
+-----------------------------+
| DirectorioTelefonico        |
| GameScores                  |
| HockeyGame                  |
| HockeyTeam                  |
| HockeyTeamPlayer            |
| Letras                      |
| RoundStats                  |
| User                        |
| UserInfo                    |
| UserScorePicks              |
| UserStatsPicks              |
| detalle_horario             |
| horario                     |
| plantilla_detalle_horario   |
| playoffround                |
| usuarios                    |
+-----------------------------+
16 rows in set (0.00 sec)
mysql>    
mysql>  INSERT INTO DirectorioTelefonico (CustomerID,TypePhone,Number)
    ->      VALUES
    ->      ('1001','Celular','333-897-5421'),
    ->      ('1001','Trabajo','333-897-6542'),
    ->      ('1001','Casa','333-698-9874'),
    ->      ('2002','Celular','333-963-6544'),
    ->      ('2002','Trabajo','333-812-9856'),
    ->      ('3003','Casa','333-987-6541');
Query OK, 6 rows affected (0.01 sec)
Records: 6  Duplicates: 0  Warnings:
