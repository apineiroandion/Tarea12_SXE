# Tarea 12 SXE
## Angel Jose Piñeiro Andion

---

## Apartado 1

### Enunciado

Como mencionamos en clase, aunque no es recomendable, en ocasiones puede ser
necesario crear tablas ajenas a Odoo dentro de su base de datos (integración con
sistemas externos, almacenamiento de históricos, datos temporales…). Mediante la
herramienta PgAdmin u otro método que estimes oportuno, elabora y ejecuta una
sentencia que cree una tabla llamada “EmpresasFCT“con los siguientes campos:

- idEmpresa: autonumérico. Este campo será la clave primaria.
- nombre: Texto con tamaño máximo de 40 caracteres. -useChatgpt: booleano, por defecto a true
- quiereAlumnos: Booleano.
- numAlumnos: número entero.
- fechaContacto: tipo fecha


    CREATE TABLE public.EmpresasFCT (
    idEmpresa SERIAL PRIMARY KEY,
    nombre VARCHAR(40),
    quiereAlumnos Boolean,
    numAlumnos integer,
    fechaContacto date
    );

Para comprobar que la tabla se haya creado correctamente ejecutamos el siguiente comando:

    select * from EmpresasFCT;

![Screenshot_20250130_130909.png](img/Screenshot_20250130_130909.png)

---

## Apartado 2

### Enunciado

Inserta 5 registros inventados en la tabla a través de una sentencia SQL.

    INSERT INTO public.EmpresasFCT (nombre, quiereAlumnos, numAlumnos, fechaContacto) VALUES
    ('Empresa1', true, 5, '2022-01-30'),
    ('Empresa2', false, 0, '2022-01-30'),
    ('Empresa3', true, 3, '2022-01-30'),
    ('Empresa4', false, 0, '2022-01-30'),
    ('Empresa5', true, 2, '2022-01-30');

![Screenshot_20250204_094436.png](img/Screenshot_20250204_094436.png)

Comprobamos que se hayan insertado correctamente los registros:

    select * from EmpresasFCT;

![Screenshot_20250204_094535.png](img/Screenshot_20250204_094535.png)









