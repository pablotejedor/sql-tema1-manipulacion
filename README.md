# sql-tema1-manipulacion

## Ejercicio 1:

CREATE TABLE curso (

 codigo INT NOT NULL,

 nombre VARCHAR(50) NOT NULL,

 descripcion VARCHAR(50),

 turno VARCHAR(50) NOT NULL,
 
 PRIMARY KEY(codigo)

);

## Ejercicio 2:

ALTER TABLE curso 
ADD cupo INT NOT NULL DEFAULT 20

## Ejercicio 3:

INSERT INTO curso (codigo, nombre, descripcion, turno, cupo)
VALUES(101, "Algoritmos", "Algoritmos y Estructuras de Datos", "Mañana", 35)

INSERT INTO curso (codigo, nombre, descripcion, turno, cupo)
VALUES(102, "Matemática Discreta", "", "Tarde", 30)

## Ejercicio 4:

INSERT INTO curso (codigo, descripcion, turno, cupo)
VALUES(109, "", "Tarde", 30)
![Captura de pantalla 2021-12-07 202618](https://user-images.githubusercontent.com/64474390/145126643-5a596832-6b1d-4472-83f4-7516dd313723.png)

## Ejercicio 5:

INSERT INTO curso (codigo, nombre, descripcion, turno, cupo)
VALUES(101, "Física", "Introducción a la Física", "Tarde", 30)
![Captura de pantalla 2021-12-07 202808](https://user-images.githubusercontent.com/64474390/145126695-7ce944ed-e4bc-49d2-8e05-c49535259d13.png)


## Ejercicio 6:

UPDATE curso
SET cupo = 25

## Ejercicio 7:

DELETE FROM curso WHERE codigo = 101
