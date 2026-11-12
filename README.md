# Recordatorio al salir

Proyecto independiente para recordar un objeto importante, como una botella o tarjeta, cuando se retiran las llaves del lugar habitual junto a la puerta. El mecanismo de detección todavía está abierto.

## Estado

Definición inicial. Sin sensor, ubicación ni prototipo validados.

## Primer alcance

- Detectar que las llaves fueron retiradas de un lugar habitual.
- Presentar el recordatorio configurado a tiempo para verlo antes de salir.
- Restablecer la espera cuando las llaves regresen.
- Evitar que una lectura incierta se presente como certeza.

La retirada de las llaves es el disparador propuesto para el piloto. La utilidad del momento se comprobará en la ubicación elegida; no se presupone un sensor de salida adicional.

## Documentos

- [Especificación del piloto](specs/001-recordatorio-llaves/spec.md).
- [Método y arquitectura compartida](docs/metodologia.md).
- [Coordinación general en Notion](https://app.notion.com/p/416504754f0881afaaa6e4297e39c813).

## Próximas decisiones

Definir el lugar de las llaves, el sensor, el tipo de aviso, la alimentación y el montaje. La conexión a la pantalla central se decidirá solo si aparece un caso de uso claro.
