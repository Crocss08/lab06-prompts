# Bitacora de prompts

- [Bitacora de prompts](prompts/BITACORA.md)

Laboratorio 06: Fundamentos de Ingenieria de Prompts. Herramienta de IA usada: (escribe aqui cual usaste) 

## Ejercicio 2: Tokens y ventana de contexto

| Texto | Caracteres | Tokens |
|---|---|---|
| Los estudiantes programan en Java. | 35 | 7 |
| The students program in Java. | 31 | 7 |
| desafortunadamente | 18 | 4    |



## Ejercicio 3: Temperatura

| Temperatura | % de BiblioTec | Nombres en los 5 intentos |
|-------------|----------------|---------------------------|
| 0 | 100.0% | LibroYa, PrestaLibro, LectoGo, PaginaLibre,NubeDeTinta |
| 0.5 | 65.3% | LibroYa, PrestaLibro, LectoGo, PaginaLibre,NubeDeTinta |
| 1 | 44.5% | LibroYa, PrestaLibro, LectoGo, PaginaLibre,NubeDeTinta |
| 1.8 | 32.2% | LibroYa, PrestaLibro, LectoGo, PaginaLibre,NubeDeTinta |


## Ejercicio 4: Prompt vago vs estructurado 

| Criterio | Prompt vago | Prompt estructurado |
|----------|-------------|---------------------|
| Menciona el objetivo del sistema | no | si |
| Menciona a los usuarios principales | no | si |
| Tiene exactamente 3 funcionalidades | no | si |
| Esta en 3 parrafos | no | si |    
| Lo usaria en un informe real | no | si |


## Ejercicio 5: Anatomia de un prompt

| Componente | Texto de mi prompt |
|------------|--------------------|
| Rol |Actua como desarrollador Java. Crea un programa en Java.|
| Instruccion |usando una clase Producto con los atributos codigo, nombre, precio y stock.|
| Contexto | Actua como desarrollador Java. Crea un programa en Java para gestionar los productos de una tienda.|
| Ejemplo | Usa este estilo para los metodos: getPrecio(), setPrecio(double precio). |
| Formato |Explica primero la estructura de la clase y luego presenta el codigo Java. |



## Ejercicio 6: Del prompt basico al profesional

```

- Actua como desarrollador

Java. Crea un ejemplo de login para una aplicacion de escritorio utilizando

Swing. El usuario debe ingresar correo y contrasena. Explica brevemente el funcionamiento y presenta

el codigo organizado por clases. 


-  Mejora el codigo anteriorcon estas restricciones: no uses librerias externas, valida que el correo

contenga @ y que la contrasena tenga al menos 8 caracteres, y muestra los

mensajes con JOptionPane.
```
<<<<<<< HEAD
[Tarea: mi prompt profesional](prompts/TAREA.md)
=======
>>>>>>> d6d595775442b8d29e83f1c8a15db25368614742
