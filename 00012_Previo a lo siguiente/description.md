Ya te presentamos las funciones `opuesto`, `previo` y `siguiente` que nos permiten desplazarnos en forma relativa a alguna dirección :exploding_head:. Antes de seguir utilizándolas, vamos a conocerlas un poco mejor.

Si partimos de este tablero inicial:

<img src="https://raw.githubusercontent.com/sagrado-corazon-alcal/mumuki-guia-fundamentos-primeros-programas-2020/master/assets/Ejemplo1_1613666233954.png" alt="Tablero de dos por dos con el cabezal en el extremo Noroeste" width="auto" height="auto">

Y luego ejecutamos `Mover(siguiente(Norte))` el tablero obtenido será así:

<img src="https://raw.githubusercontent.com/sagrado-corazon-alcal/mumuki-guia-fundamentos-primeros-programas-2020/master/assets/Ejemplo2_1613666255883.png" alt="Tablero de dos por dos con el cabezal en el extremo Noreste" width="auto" height="auto">

Porque `siguiente(Norte)` es `Este`. Si luego ejecutamos `Mover(previo(Oeste))` lograremos el siguiente tablero:

<img src="https://raw.githubusercontent.com/sagrado-corazon-alcal/mumuki-guia-fundamentos-primeros-programas-2020/master/assets/Ejemplo3_1613666275495.png" alt="Tablero de dos por dos con el cabezal en el extremo Sureste" width="auto" height="auto">

Porque `previo(Oeste)` es `Sur`. ¡Veamos si se entendió! :smiley: 

> Si tenemos este tablero inicial:
>
> <img src="https://raw.githubusercontent.com/sagrado-corazon-alcal/mumuki-guia-fundamentos-primeros-programas-2020/master/assets/TableroInicial_1613666173929.png" alt="Tablero de tres por tres con el cabezal en el extremo Noroeste" width="auto" height="auto">
>
> ¿Qué tablero se consigue luego de invocar el siguiente procedimiento?
>
>```gobstones
procedure PonerMisterioso() {
  Mover(siguiente(Este))
  Poner(Negro)
  Mover(opuesto(Oeste))
  Poner(Negro)
  Mover(previo(Oeste))
  Poner(Negro)
}