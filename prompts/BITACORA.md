# Bitacora de prompts
 
Laboratorio 06: Fundamentos de Ingenieria de Prompts.
 
Herramienta de IA usada: (escribe aqui cual usaste)
 
## Ejercicio 2: Tokens y ventana de contexto
 
## Ejercicio 3: Temperatura
 
## Ejercicio 4: Prompt vago vs estructurado
 
## Ejercicio 5: Anatomia de un prompt
 
## Ejercicio 6: Del prompt basico al profesional


| Texto | Caracteres | Tokens |
|---|---|---|
| Los estudiantes programan en Java. | 36 | 7 |
| The students program in Java. | 29 | 6 |
| desafortunadamente | 18 | 4 |


| Temperatura | % de BiblioTec | Nombres en los 5 intentos |
|---|---|---|
| 0 | 100.0% | BiblioTec, BiblioTec, BiblioTec, BiblioTec, BiblioTec |
| 0.5 | 65.3% | PrestaLibro, BiblioTec, LibroYa, BiblioTec, BiblioTec |
| 1 | 44.5% | LibroYa, PaginaLibre, BiblioTec, BiblioTec, LibroYa |
| 1.8 | 32.2% | LibroYa, PrestaLibro, BiblioTec, BiblioTec, PrestaLibro |


| Criterio | Prompt vago | Prompt estructurado |
|---|---|---|
| Menciona el objetivo del sistema | Sí | Sí |
| Menciona a los usuarios principales | No | Sí |
| Tiene exactamente 3 funcionalidades | No | Sí |
| Esta en 3 parrafos | No | Sí |
| Lo usaria en un informe real | No | Sí |



| Componente | Texto de mi prompt |
|---|---|
| Rol | Actua como desarrollador Java |
| Instruccion | Crea un programa en Java ... usando una clase Producto con los atributos codigo, nombre, precio y stock |
| Contexto | para gestionar los productos de una tienda |
| Ejemplo | Usa este estilo para los metodos: getPrecio(), setPrecio(double precio) |
| Formato | Explica primero la estructura de la clase y luego presenta el codigo Java |


- Nivel 1: La IA creó un programa genérico (probablemente un "Hola Mundo" o una calculadora básica).
- Nivel 2: Al darle el rol, el código tuvo mejores prácticas y comentarios de un desarrollador.
- Nivel 3: Al agregar el contexto, el programa se enfocó en productos de una tienda en lugar de ser genérico.
- Nivel 4: Al especificar la clase Producto y sus atributos, la IA dejó de adivinar y creó exactamente lo que pedí.
- Nivel 5: Al pedir el formato, la IA explicó la estructura antes del código, lo que hace más fácil entenderlo.


| Qué revisar | Cumple (Sí / No) |
|---|---|
| ¿Está escrito en Java y usa Swing? | Sí |
| ¿Pide correo y contraseña? | Sí |
| ¿Explica el funcionamiento antes o después del código? | Sí |
| ¿El código está organizado en clases? | Sí |
| ¿Valida los datos que ingresa el usuario? | Sí (pero solo valida que no estén vacíos) |


```text
Mejora el codigo anterior con estas restricciones: no uses librerias
externas, valida que el correo contenga @ y que la contrasena tenga
al menos 8 caracteres, y muestra los mensajes con JOptionPane.
```

