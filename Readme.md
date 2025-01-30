
## Apartado 1

![Screenshot_20250130_130306.png](../../../../tmp/Spectacle.whMBCQ/Screenshot_20250130_130306.png)

    CREATE TABLE public.EmpresasFCT (
    idEmpresa SERIAL PRIMARY KEY,
    nombre VARCHAR(40),
    quiereAlumnos Boolean,
    numAlumnos integer,
    fechaContacto date
    );

![Screenshot_20250130_130716.png](../../../../tmp/Spectacle.whMBCQ/Screenshot_20250130_130716.png)

Para comprobar que la tabla se haya creado correctamente ejecutamos el siguiente comando:

    select * from EmpresasFCT;

![Screenshot_20250130_130909.png](../../../../tmp/Spectacle.whMBCQ/Screenshot_20250130_130909.png)





