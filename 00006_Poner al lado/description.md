Para ver si entendiste lo anterior, te toca ahora resolver por tu cuenta.

Queremos hacer un procedimiento que nos sirva para poner una bolita **al lado** de donde se encuentre el cabezal, dejándolo en la posición original. Por ejemplo, al usar `PonerAl(Norte, Verde)` debería poner una bolita verde una posición hacia el Norte, **sin mover** el cabezal (bueno, ya sabemos que en realidad sí se mueve, pero el punto es que en el **resultado final** esto no se tiene que ver).

<table class= "table" style="width:100%">
  <thead>
  <tr>
    <th style="text-align: center">Inicial</th>
    <th style="text-align: center"></th> 
    <th style="text-align: center">Final</th>
  </tr>
  </thead>
  <tbody>
  <tr>
    <td style="text-align: center">  
      <gs-board>
        GBB/1.0
        size 2 2
        head 1 0
      </gs-board>
    </td>
    <td style="text-align: center"><i class="fa fa-arrow-right"></i></td> 
    <td style="text-align: center">
      <gs-board>
        GBB/1.0
        size 2 2
        cell 1 1 Verde 1
        head 1 0
      </gs-board>
    </td>
  </tr>
  <tbody>
</table>

> Desarrollá el procedimiento `PonerAl(direccion, color)` que resuelva el problema propuesto.