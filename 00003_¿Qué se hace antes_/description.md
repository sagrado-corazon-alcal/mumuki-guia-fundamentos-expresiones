De un conocido diario (no podemos revelar su nombre por temas de confidencialidad) nos pidieron desarrollar un procedimiento para contar, aproximadamente, cuánta gente asistió a una determinada manifestación.

Contamos con la información de cuántos micros, autos y bicicletas asistieron y desde allí podemos hacer un cálculo siguiendo estas reglas:

* en cada **micro** viajan **40 personas**;
* en cada **auto** viajan **4 personas**;
* en cada **bicicleta** viaja **1 persona**.

> Implementá el procedimiento `ContarGente(micros, autos, bicicletas)` que a partir de la cantida de micros, autos y bicicletas que recibe como parámetro, haga las cuentas necesarias y refleje el resultado con bolitas de color verde.

Te dejamos un par de ejemplos que te pueden ayudar:

* `ContarGente(1, 1, 1)` generaría este tablero:

<gs-board>
  GBB/1.0
  size 2 2
  cell 0 0 Verde 45
  head 0 0     
</gs-board>

* `ContarGente(1, 2, 3)` generaría este tablero:

<gs-board>
  GBB/1.0
  size 2 2
  cell 0 0 Verde 51
  head 0 0     
</gs-board>
