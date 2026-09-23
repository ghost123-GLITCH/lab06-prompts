# Tarea: Mi prompt profesional

## Funcionalidad elegida
Registro de clientes para una tienda.

## Version 1: prompt basico
```text
Hazme un programa para registrar clientes.
```
**Qué cambie:** Nada, fue el punto de partida.
**Por que:** Quería ver qué tan genérica era la respuesta de la IA sin darle ninguna dirección.
**Qué mejoro:** La IA generó un código muy básico, en un lenguaje que no especifiqué y sin estructura clara. Confirmé que un prompt vago da un resultado impredecible.

## Version 2
```text
Actua como desarrollador Java. Crea un programa para registrar clientes de una tienda, usando una clase Cliente con los atributos dni, nombre, correo y telefono.
```
**Qué cambie:** Agregué el rol (desarrollador Java) y el contexto (tienda), además de especificar la clase Cliente y sus atributos.
**Por que:** La versión 1 fue demasiado general. Necesitaba que la IA supiera el lenguaje y la estructura de datos que quería.
**Qué mejoro:** La IA dejó de adivinar. Creó código en Java con la clase Cliente exacta que pedí, pero aún no organizaba el código ni explicaba cómo usarlo.

## Version 3: prompt final
```text
Actua como desarrollador Java senior. Crea un sistema de registro de clientes para una tienda, usando una clase Cliente con los atributos dni, nombre, correo y telefono. El sistema debe permitir agregar clientes, listarlos y buscarlos por DNI. Explica primero la estructura de las clases y luego presenta el codigo Java completo organizado por clases. Usa este estilo para los metodos: getNombre(), setNombre(String nombre). Restriccion: no uses librerias externas, solo la libreria estandar de Java.
```

### Explicación de la iteración final
**Qué cambie:** Agregué instrucciones específicas (agregar, listar, buscar), el formato de salida (explicar estructura y luego código), un ejemplo de estilo de métodos y una restricción clara.
**Por que:** La versión 2 funcionaba, pero el código no estaba organizado ni explicado. Además, quería asegurarme de que no usara librerías externas para que fuera fácil de compilar.
**Qué mejoro:** La IA entregó un código completo, organizado en clases (Cliente, GestorClientes, Main), con explicación previa, métodos siguiendo el estilo pedido y sin dependencias externas.

## Componentes del prompt final
| Componente | Texto de mi prompt |
|---|---|
| Rol | Actua como desarrollador Java senior. |
| Instruccion | Crea un sistema de registro de clientes ... que permita agregar clientes, listarlos y buscarlos por DNI. |
| Contexto | para una tienda, usando una clase Cliente con los atributos dni, nombre, correo y telefono. |
| Ejemplo | Usa este estilo para los metodos: getNombre(), setNombre(String nombre). |
| Formato | Explica primero la estructura de las clases y luego presenta el codigo Java completo organizado por clases. |
| Restriccion | no uses librerias externas, solo la libreria estandar de Java. |

## Evaluación del resultado
| Criterio | Cumple (Sí / No) |
|---|---|
| ¿El código está en Java y usa la clase Cliente pedida? | Sí |
| ¿Permite agregar, listar y buscar clientes? | Sí |
| ¿Explica la estructura antes de mostrar el código? | Sí |
| ¿Respeta la restricción de no usar librerías externas? | Sí |
| ¿Usa el estilo de métodos solicitado (get/set)? | Sí |

## Errores frecuentes y cómo los evité

1. **Error: Ser demasiado general.**  
   En la versión 1 escribí "Hazme un programa para registrar clientes" y la IA no sabía ni el lenguaje ni la estructura.  
   **Cómo lo evité:** En la versión 3 especifiqué el rol, el lenguaje, la clase y los atributos exactos.

2. **Error: No indicar el formato.**  
   En la versión 2 el código funcionaba, pero estaba todo mezclado y sin explicación.  
   **Cómo lo evité:** En la versión 3 le pedí explícitamente "Explica primero la estructura y luego presenta el código organizado por clases".

## Enlace al repositorio
Este archivo forma parte del repositorio [lab06-prompts](https://github.com/ghost123-GLITCH/lab06-prompts).