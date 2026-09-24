# Tarea: Mi prompt profesional

## Funcionalidad elegida

Sistema de **registro de clientes** para una tienda: permite guardar nombre, correo y teléfono de cada cliente, validarlos y listarlos.

## Version 1: prompt basico

```text
Hazme un registro de clientes en Java.
```

**Qué cambié:** nada aún, es el punto de partida.
**Por qué:** quería ver qué genera la IA sin ningún componente adicional.
**Qué faltó en la respuesta:** la IA asumió sus propios atributos (algunos inventados), no explicó la estructura, no usó ningún patrón de validación y entregó el código sin contexto de uso ni organización en clases.

## Version 2

```text
Actua como desarrollador Java. Crea un sistema para registrar clientes
de una tienda, con los atributos nombre, correo y telefono, usando
una clase Cliente.
```

**Qué cambié:** agregué rol ("desarrollador Java") y contexto (para qué sirve, qué atributos usar, qué clase crear).
**Por qué:** en la Versión 1 la IA inventaba atributos distintos cada vez; quería fijar el objetivo y los datos exactos.
**Qué mejoró:** ahora la clase `Cliente` siempre tiene los tres atributos pedidos y el propósito del sistema queda claro, pero todavía no valida los datos ni explica el código antes de mostrarlo.

## Version 3: prompt final

```text
Actua como desarrollador Java. Crea un sistema de registro de clientes
para una tienda, usando una clase Cliente con los atributos nombre,
correo y telefono.

Debe incluir una clase RegistroClientes con metodos para agregar,
listar y buscar un cliente por correo.

No uses librerias externas: solo Java estandar (ArrayList, Scanner).
Valida que el correo contenga "@" y que el telefono tenga
exactamente 9 digitos.

Usa este estilo para los metodos: getNombre(), setNombre(String nombre).

Explica primero la estructura de las clases y luego presenta el
codigo Java completo.
```

## Componentes del prompt final

| Componente    | Texto de mi prompt |
|---------------|---------------------|
| Rol           | Actua como desarrollador Java. |
| Instrucción   | Crea un sistema de registro de clientes para una tienda... Debe incluir una clase RegistroClientes con métodos para agregar, listar y buscar un cliente por correo. |
| Contexto      | ...usando una clase Cliente con los atributos nombre, correo y telefono. |
| Ejemplo       | Usa este estilo para los métodos: getNombre(), setNombre(String nombre). |
| Formato       | Explica primero la estructura de las clases y luego presenta el código Java completo. |
| Restricción   | No uses librerías externas: solo Java estándar (ArrayList, Scanner). Valida que el correo contenga "@" y que el teléfono tenga exactamente 9 dígitos. |

## Evaluacion del resultado

| Qué revisar                                         | Cumple (Sí/No) |
|------------------------------------------------------|----------------|
| ¿Está escrito en Java estándar, sin librerías externas? | si |
| ¿La clase Cliente tiene los tres atributos pedidos?   | si |
| ¿Valida correo y teléfono como se pidió?             | si |
| ¿Explica la estructura antes del código?             | si |
| ¿Los métodos siguen el estilo get/set indicado?      | si |

*(Marca cada fila con Sí o No después de probar el prompt en tu asistente de IA.)*

## Errores que evité

- **Ser demasiado general:** en la Versión 1 no había rol ni contexto, por lo que la IA tuvo que adivinar los atributos del cliente. Lo evité agregando rol y contexto explícito desde la Versión 2.
- **No indicar el formato:** en las primeras versiones no pedí un orden de presentación, así que la IA mezclaba explicación y código sin criterio. Lo evité pidiendo explícitamente "explica primero la estructura y luego el código" en la Versión 3.