# Especificación 001: recordatorio de llaves

**Estado:** propuesta para validar.

## Propósito

Reducir la posibilidad de salir sin llaves mediante un recordatorio en el momento adecuado.

## Comportamiento esperado

1. El sistema reconoce la retirada de las llaves de un lugar fijo.
2. Se emite un recordatorio antes de la salida según una señal de salida por definir.
3. Cuando las llaves vuelven, el estado se restablece.
4. Si el estado del objeto no puede determinarse, se informa incertidumbre y no se afirma que las llaves están o no están.

## Criterios de aceptación del piloto

- Se distinguen retiro, devolución y estado desconocido.
- La devolución permite un nuevo ciclo de uso.
- El recordatorio no se repite sin límite en un mismo ciclo.
- La prueba comprueba que el aviso ocurre antes del punto en que ya es inútil.

## Fuera de alcance por ahora

Rastreo de ubicación de personas, localización remota de llaves y vínculo con la pantalla central.

## Preguntas abiertas

¿Qué constituye «salir»? ¿Qué objeto se prioriza? ¿Qué lugar fijo se usará? ¿Cómo se evita que otra persona o un cambio de rutina genere falsas conclusiones?

