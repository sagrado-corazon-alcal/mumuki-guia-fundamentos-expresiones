Bueno, basta de números (por un ratito). Ahora vamos a aprender a hacer "cuentas" con las direcciones.

Para hacer esto, simularemos el movimiento de un salmón: en contra de la corriente. Nuestro objetivo será escribir un procedimiento `MoverComoSalmon(direccion)` que reciba una dirección y se mueva exactamente una vez en la dirección **opuesta**. Veamos en una tabla cómo debería comportarse este procedimiento:

* `MoverComoSalmon(Norte)` <i class="fa fa-arrow-right"></i> se mueve hacia el **Sur**.
* `MoverComoSalmon(Este)` <i class="fa fa-arrow-right"></i> se mueve hacia el **Oeste**.
* `MoverComoSalmon(Sur)` <i class="fa fa-arrow-right"></i> se mueve hacia el **Norte**.
* `MoverComoSalmon(Oeste)` <i class="fa fa-arrow-right"></i> se mueve hacia el **Este**.

Como la dirección va a ser un parámetro de nuestro procedimiento, necesitamos una forma de decir _"la dirección opuesta a X"_ para poder luego usar esto como argumento de `Mover`. Gobstones nos provee un mecanismo para hacer esto, la primitiva `opuesto(dir)`. En criollo: `opuesto` (¡sí, en minúsculas!) nos dice la dirección contraria a la `dir` que nosotros le pasemos.

Sabiendo esto, podríamos implementar fácilmente el procedimiento que queríamos:

```gobstones
procedure MoverComoSalmon(direccion) {
  Mover(opuesto(direccion))
}
```

> Escribí la solución en el editor y dale Enviar. Vas a ver cómo se mueve el cabezal...