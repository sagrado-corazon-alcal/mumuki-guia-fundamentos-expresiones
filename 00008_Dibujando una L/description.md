Nuestro objetivo en este ejercicio será realizar un procedimiento capaz de dibujar una letra L de color Azul, pero con la posibilidad de elegir hacia dónde está orientada. A continuación, algunos ejemplos de cómo debería comportarse:

|Ele(Norte)|Ele(Este)|
|----------|---------|
|![Ele(Norte)](https://raw.githubusercontent.com/sagrado-corazon-alcal/mumuki-guia-fundamentos-expresiones/master/images/ele-norte.png)|![Ele(Este)](https://raw.githubusercontent.com/sagrado-corazon-alcal/mumuki-guia-fundamentos-expresiones/master/images/ele-este.png)|

Indudablemente, una L consta de dos líneas y dibujar una línea es la tarea que ya resolviste en el ejercicio anterior. Así que por ese lado, tenemos la mitad del problema resuelto.

La primera línea es fácil, porque coincide con la dirección que recibimos por parámetro... ¿pero la segunda? Bueno, ahí viene lo interesante: además de `opuesto`, Gobstones nos provee dos funciones más para operar sobre las direcciones, `siguiente` y `previo`.

> Escribí el procedimiento `Ele(direccion)` que haga lo pedido.