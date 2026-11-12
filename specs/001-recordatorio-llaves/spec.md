# Especificación 001: recordatorio al retirar las llaves

**Estado:** propuesta para validar. No hay sensor, montaje ni prototipo físico verificados.

## Propósito

Recordar un objeto elegido por la persona (por ejemplo, botella o tarjeta) en el momento de tomar las llaves para salir del departamento.

## Escena de uso

Las llaves descansan en un lugar habitual junto a la puerta. Al retirarlas, el objeto presenta un recordatorio configurable que puede verse antes de salir. Cuando las llaves regresan, queda listo para el siguiente ciclo.

## Primer comportamiento

1. **Espera:** las llaves se consideran presentes y no hay recordatorio de salida activo.
2. **Retirada confirmada:** se presenta el recordatorio configurado una vez para ese ciclo.
3. **Llaves ausentes:** el recordatorio no se dispara repetidamente mientras continúan ausentes.
4. **Devolución confirmada:** se retira el aviso y el sistema vuelve a espera.
5. **Estado desconocido:** si la detección es inconclusa, el sistema no afirma que las llaves están presentes ni ausentes. La forma de mostrar o registrar esta incertidumbre se decidirá con la interfaz.

La retirada de llaves es el disparador propuesto para el piloto; no se presupone un segundo sensor que detecte la salida.

## Criterios de aceptación del piloto

- Una retirada confirmada activa el recordatorio configurado sin otra acción.
- La devolución confirmada restablece la espera y permite un nuevo ciclo.
- El aviso se activa una sola vez por ciclo; no se repite sin límite mientras las llaves siguen fuera.
- Las lecturas inconclusas no se cuentan como retiradas o devoluciones correctas.
- En una prueba en la ubicación elegida, el aviso resulta perceptible antes de abrir la puerta y el objeto no estorba el movimiento habitual de las llaves ni de la puerta.
- La prueba registra retiradas, devoluciones y movimientos de las llaves que no constituyen una retirada, junto con aciertos, omisiones y avisos falsos.

## Fuera de alcance por ahora

Rastreo de personas, localización remota de llaves, detección independiente de apertura de puerta y vínculo con la pantalla central.

## Decisiones abiertas

- Lugar habitual de las llaves y ubicación del objeto.
- Método de detección y tratamiento de lecturas ambiguas.
- Tipo de aviso, forma física y alimentación.
- Contenido inicial del recordatorio y modo de configurarlo.
- Umbral aceptable de omisiones y avisos falsos tras las primeras pruebas.

## Evidencia pendiente

Primero se debe comprobar la escena de uso y el espacio disponible. Después se compararán sensores con un montaje de prueba y se registrarán los resultados. Ninguna de esas pruebas se ha realizado todavía.
