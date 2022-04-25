## Mysql basic instructions
* Create table
```sql
CREATE TABLE `Usuario` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `username` varchar(50) CHARACTER SET utf8mb3 DEFAULT NULL,
  `email` varchar(50) CHARACTER SET utf8mb3 DEFAULT NULL,
  `edad` int(3) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=5 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_unicode_ci
);
```
* SELECT
```sql
SELECT * FROM prueba.Usuario;
```
* ALTER TABLE
```sql
ALTER TABLE Usuario ADD edad INT;
```
```sql
ALTER TABLE Usuario DROP COLUMN edad;
```
```sql
ALTER TABLE Usuario MODIFY COLUMN email VARCHAR(50);
```
* INSER INTO
```sql
INSERT INTO Usuario (email, username)
  VALUES('correo@gmail.com', 'user');
```
* DELETE
```sql
DELETE FROM Usuario WHERE email = 'correo@gmail.com' LIMIT 1;
```
* ALTER TABLE
```sql
ALTER TABLE Usuario ADD PRIMARY KEY (id);
```
```sql
ALTER TABLE Usuario MODIFY COLUMN id INT AUTO_INCREMENT;
```
* SELECT 
```sql
SELECT * FROM Usuario;
```
```sql
SELECT * FROM Usuario WHERE email = 'correo2@gmail.com';
```
* UPDATE
```sql
UPDATE Usuario SET edad = 18 WHERE id = 1;
```
* DELETE
```sql
DELETE FROM Usuario WHERE id = 4;
```

 # Créditos
  [J. Hernandez](https://github.com/Jorge-E-HH) autor original del contenido.
