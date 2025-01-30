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



