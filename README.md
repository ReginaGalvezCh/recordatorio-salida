# Recordatorio al salir

Proyecto independiente para recordar un objeto importante, inicialmente las llaves, antes de abandonar un lugar. El mecanismo de detección todavía está abierto.

## Estado

Definición inicial. Sin sensor, ubicación ni prototipo validados.

## Primer alcance

- Detectar que las llaves fueron retiradas de un lugar habitual.
- Dar un recordatorio oportuno antes de salir.
- Restablecer el estado cuando las llaves regresen.
- Evitar que un fallo de detección se presente como certeza.

## Documentos

- [Especificación del piloto](specs/001-recordatorio-llaves/spec.md).
- [Método y arquitectura compartida](docs/metodologia.md).

## Próximas decisiones

Definir el momento exacto en que el recordatorio es útil, el lugar de las llaves y cómo reconocer retiro, regreso y salida. La conexión a la pantalla central se decidirá solo si aparece un caso de uso claro.

