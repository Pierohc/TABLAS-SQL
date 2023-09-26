## Datos:
SQL es una base de datos relacional.

## Estructura: 

Las columnas son los atributos(mismo tipo de dato).

Las filas o registros son llamadas tuplas, en si son los objetos.

|   NOMBRE      |      DNI        |    NACIMIENTO |
|---------------|-----------------|---------------|
|Juan Perez     |     12345678    |    20/03/1999 |
|Carlos García  |     87654321    |    15/06/1970 |

## Modelado de Base de Datos:
Lo de la derecha es una tabla
![image](https://github.com/Pierohc/DB-SQL/assets/133154904/d53e35cc-a665-4deb-bbca-88b58b384094)

## Tipos de datos: 
En toda tabla siempre habrá una  ***primary key (PK)*** ![image](https://github.com/Pierohc/DB-SQL/assets/133154904/e40bbd66-0393-4edb-a823-7fe620016f3e), pueden haber mas, está permite identificar univocamente a cada fila, esta no se puede repetir. 


## Rombo celeste sin colorear:
Significa que esa columna puede ser nula.

Por ejemplo si nombre y nacimiento tiene un rombo celeste sin colorear, significa que puedo crear una persona solo con DNI, sin nombre y sin fecha de nacimiento.

## Rombo celeste coloreado:
Si queremos que un campo sea obligatorio debemos ponerlo NN(No Null).

## Rombo rojo sin colorear:
Un foreign key que puede ser null. En el origne de la conexión habrá un |o

## Rombo rojo coloreado:
Un foreign key que no puede ser null. En el origne de la conexión habrá un ||


## Enteros: 
![image](https://github.com/Pierohc/DB-SQL/assets/133154904/71301110-94c4-4fc4-81f0-54bbc4d8ef19)

## Decimales:
Si tengo 6.555 y coloco double(2) este sera 6.55, por ello en temas financieros es mejor usar decimal
![image](https://github.com/Pierohc/DB-SQL/assets/133154904/62b4823a-112d-4b56-a742-a21c66c4e1fc)

## Fecha:
![image](https://github.com/Pierohc/DB-SQL/assets/133154904/7cd66190-7bf1-48ac-a854-90764f2859fc)
Cabe resaltr que si NO vamos a realizar alguna operación matemática con le fecha, lo mejor será guardarla como String.

## Cadena de caracteres: 
![image](https://github.com/Pierohc/DB-SQL/assets/133154904/fce58d44-c1bb-41e3-8c45-2e122fb46674)
Char se usa cuando estamos seguros del tamaño de lo que se va a guardar.

Varchar cuando no estamos seguros de tamaño, este es variable.

-------------------------------
## Modelo entidad relación: 
![image](https://github.com/Pierohc/DB-SQL/assets/133154904/1c7b2db0-943f-4f68-a8e4-fce69f2e8611)

## Foreign Key (Llave foranea):
Cuando pasamos una primary key de una tabla a otra esta se llamada foreign key(FK)
![image](https://github.com/Pierohc/DB-SQL/assets/133154904/54722aeb-83a7-4c78-b32e-b251d2bf8270)

----

## Conexiones:
Uno a muchos: 
![image](https://github.com/Pierohc/DB-SQL/assets/133154904/f0f1ebc8-dad2-4834-8541-2280a68e4ff5)

----
Una relacion es ***fuerte*** cuando la tabla es dependiente, en este caso el celular se vuelve dependiente de la persona. Por asi decirlo, si imaginamos que no hay ninguna personas, no podriamos crear un celular.
Y en ese caso cuando le paso la PK de persona, tambien pasaria a ser la PK de celular. Y tendriamos una PK compuesta(puede de 2 a más). Significada que el par o más llave representa a la tabla.

Cuando la relación es ***debil*** si estariamos pasando una foreign key (FK) y esa PK pasaria a ser una columna más.

Lo mejor será modelar con conexiones débiles

---------------------------------------------------
# BASE DE DATOS:









