## Errores encontrados en la consola del navegador

**Detalle:** La App no validaba ningun dato ingresado, no realizaba ninguna accion
**Error:** El metodo addEventListener  fue escrito de forma incorrecta, con minuscula la segunda palabra del metodo
**Linea:** 87 

**Detalle:** La aplicacion ya recibe los digitos pero no realiza ninguna validacion
**Error:** Se corrige linea 49 en donde el elemento con clase .lowOrHi, no habia sido registrado con el punto y en la linea 77 y 79 se seleccionaba el elemento pero sin ser encontrado 


**Error:** El metodo addEventListener del resetButton fue escrito de forma incorrecta, con minuscula la segunda palabra del metodo
**Linea** 95


## Errores de logica detectados en codigo 

**Detalle:** La aplicacion acepta codigos decimales, en una prueba detecto que el numero correcto es 7.5
**Error:** en la linea 44 se declara ramdaomNumber como numero aleatorio pero es tipo flotante poo lo que puede aceptar cualquier tipo de dato decimal, se corrige por la funcion Math.floor(Math.random() * 100) + 1; que gararantiza que el numero sea entre 1 y 100

**Detalle:** la aplicacion al quinto intento indica que es correcto.
**Error:** Se encuentra que se declaro una constante ATTEMPTS = 5, Que indica que son 5 intentos, Se modifica la declaracion de la constante a 10.
**Linea:** 46


