# Ejemplo de Aplicación de Proceso de Pago

Este es un ejemplo de una aplicación de proceso que contiene un proceso de pago y los trabajadores, formularios y servicios ficticios necesarios.

Puede usar la imagen generada a partir de esta aplicación Spring Boot para tener el primer ejemplo en ejecución en su instalación autogestionada de un clúster de Camunda 8.

## Características

- Despliegue automático del archivo BPMN al iniciar la aplicación.
- Formulario para iniciar instancias de proceso manualmente.
- API REST para iniciar instancias de proceso (programada por usted).
- Trabajadores con lógica de negocio incluida.

###
Ejemplo en test.http

## Interacción con la lógica de negocio

La aplicación escribe la interacción de las instancias de proceso con la lógica de negocio en el registro del contenedor. Allí encontrará un resultado como este:

```
Gestionando crédito de cliente para la instancia de proceso 2251799813720515
El cliente cust50 tiene un crédito de 50.0
Se cargaron 50.0 del crédito, el importe pendiente es de 17.5
Gestionando pago con tarjeta de crédito para la instancia de proceso 2251799813720515
Se carga la tarjeta 1234 4567 que vence el 24/12 y tiene el CVC 123 con un importe de 17.5
Pago completado
```
