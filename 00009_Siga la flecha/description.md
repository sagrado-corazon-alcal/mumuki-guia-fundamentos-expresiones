Ya vimos distintas funciones que a partir de una dirección nos permiten obtener otra distintas. 

Como siempre en programación, lo interesante es combinar nuestras herramientas para lograr nuevos objetivos :sunglasses:. Por ejemplo podemos dibujar flechas en una dirección determinada de la siguiente forma:

<table class= "table" style="width:100%">
  <thead>
  <tr>
    <th style="text-align: center">Flecha(Norte)</th>
    <th style="text-align: center"></th> 
    <th style="text-align: center">Flecha(Oeste)</th>
  </tr>
  </thead>
  <tbody>
  <tr>
    <td style="text-align: center">  
      <gs-board>
        GBB/1.0
        size 3 3
        cell 1 2 Rojo 1
        cell 0 1 Rojo 1
        cell 2 1 Rojo 1
        head 1 1
      </gs-board>
    </td>
    <td style="text-align: center"></td> 
    <td style="text-align: center">
      <gs-board>
        GBB/1.0
        size 3 3
        cell 1 2 Rojo 1
        cell 0 1 Rojo 1
        cell 1 0 Rojo 1
        head 1 1
      </gs-board>
    </td>
  </tr>
  <tbody>
</table>

> Definí el procedimiento `Flecha(direccion)` que dibuje una flecha roja en la dirección correspondiente. El cabezal empieza y debe quedar siempre en el centro, como se ve en las imágenes.
