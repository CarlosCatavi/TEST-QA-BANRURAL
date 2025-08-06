## ------------ Errores encontrados en la consola del navegador

**Detalle:** La App no validaba ningun dato ingresado, no realizaba ninguna accion
**Error:** El metodo addEventListener  fue escrito de forma incorrecta, con minuscula la segunda palabra del metodo
**Linea:** 87 

**Detalle:** La aplicacion ya recibe los digitos pero no realiza ninguna validacion
**Error:** Se corrige linea 49 en donde el elemento con clase .lowOrHi, no habia sido registrado con el punto y en la linea 77 y 79 se seleccionaba el elemento pero sin ser encontrado 


**Error:** El metodo addEventListener del resetButton fue escrito de forma incorrecta, con minuscula la segunda palabra del metodo
**Linea** 95


## ------------- Errores de logica detectados en codigo 

**Detalle:** La aplicacion acepta codigos decimales, en una prueba detecto que el numero correcto es 7.5
**Error:** en la linea 44 se declara ramdaomNumber como numero aleatorio pero es tipo flotante poo lo que puede aceptar cualquier tipo de dato decimal, se corrige por la funcion Math.floor(Math.random() * 100) + 1; que gararantiza que el numero sea entre 1 y 100

**Detalle:** la aplicacion al quinto intento indica que es correcto.
**Error:** Se encuentra que se declaro una constante ATTEMPTS = 5, Que indica que son 5 intentos, Se modifica la declaracion de la constante a 10.
**Linea:** 46


**Detalle:** La aplicacion ya valida los 10 intentos pero continua el problema, al 10mo intento indica que es el numero correcto.
**Error:** Se identifica que los mensajes estan cruzados en la linea indica: Perdiste!! pero deberia ser: 'Felicitaciones! adivinaste el número!'
y en la linea 70 idica: 'Felicitaciones! adivinaste el número!' pero deberia ser:  Perdiste!!

**Detalle:** El programa ya valida y lanza un mensaje de que perdio al finalizar el ultimo intento, pero se observa que el mensaje donde indica si el numero es mayor o menor,
**Error:** Los mensajes de Numero es mayor, tambien esta cruzado con Numero es Menor y viceversa
**Linea:** 77 - 79

**Detalle:** Ya valida que el numero sea mayor o menor, pero se identifica que al momento de mostrar el mensaje de incorrecto! o Ganaste, Resalta un color para cada mensaje.
**Error:** Se identifica que la etiqueta para cada texto estan cruzadas, para el texto Incorrecto, se corrige con color red y para la Felicidades adivinaste, se corrige con green
**Linea:** 71 - 75


**Detalle:** Se verifica que en realidad nunca se acierta, puedo poner 91 y dice que es menor, pero pongo 92 y dice que es mayor.
**Error:** Se esta comparando un string con un numero decimal, por eso nunca se acierta, se corrige linea 61 y se declara let userGuess = Number(guessField.value.trim());

## -- Fin
