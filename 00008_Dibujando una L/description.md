Nuestro objetivo en este ejercicio será definir un procedimiento capaz de dibujar una letra L de color Azul, pero con la posibilidad de elegir hacia dónde está orientada. A continuación, algunos ejemplos de cómo debería comportarse:

<table class= "table table-borderless" style="width:100%">
  <thead>
  <tr>
    <th style="text-align: center">Ele(Norte)</th>
    <th style="text-align: center"></th> 
    <th style="text-align: center">Ele(Este)</th>
  </tr>
  </thead>
  <tbody>
  <tr>
    <td style="text-align: center">  
      <gs-board>
        GBB/1.0
        size 4 4
        cell 0 0 Azul 2
        cell 0 1 Azul 1
        cell 0 2 Azul 1
        cell 1 0 Azul 1
        cell 2 0 Azul 1
        head 0 0
      </gs-board>
    </td>
    <td style="text-align: center"></td> 
    <td style="text-align: center">
      <gs-board>
        GBB/1.0
        size 4 4
        cell 0 3 Azul 2
        cell 0 2 Azul 1
        cell 0 1 Azul 1
        cell 1 3 Azul 1
        cell 2 3 Azul 1
        head 0 3
      </gs-board>
    </td>
  </tr>
  <tbody>
</table>

<br>
Indudablemente, una L consta de dos líneas y dibujar una línea es la tarea que ya resolviste en el ejercicio anterior. Así que por ese lado, tenemos la mitad del problema resuelto.

La primera línea es fácil, porque coincide con la dirección que recibimos como argumento... ¿pero la segunda? Bueno, ahí viene lo interesante: además de `opuesto`, Gobstones nos provee dos funciones más para operar sobre las direcciones, `siguiente` y `previo`. `siguiente(direccion)` retorna la dirección siguiente a la especificada, mientras que `previo(direccion)` retorna la anterior, siempre pensándolo en el sentido de las agujas del reloj:

<center> <img src="https://raw.githubusercontent.com/sagrado-corazon-alcal/mumuki-guia-fundamentos-expresiones/master/images/rosa-de-los-vientos.png" width=300 alt="Rosa de los vientos que muestra que previo de Norte es Oeste y siguiente de Norte es Este"/> </center> 

> Descubrí cuál de las funciones nuevas tenés que invocar y definí el procedimiento `Ele(direccion)`. No te preocupes por la posición inicial del cabezal, nosotros nos encargaremos de ubicarlo en el lugar correspondiente para que la L se pueda dibujar.