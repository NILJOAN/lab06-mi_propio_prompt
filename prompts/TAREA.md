# Tarea: Mi prompt profesional

## Funcionalidad seleccionada
Sistema de Cálculo de Notas para Alumnos en Java.

## Iteraciones del Prompt

### Versión 1 (Prompt Básico)
```text
Crea un programa en Java para calcular notas de alumnos.
```
* **Qué cambió y por qué:** Es el punto de partida inicial. Es un prompt vago porque no tiene contexto, ni restricciones de escala ni formato.
* **Resultado de la IA:** La IA genera un código muy simple en consola con `Scanner`, sin estructura orientada a objetos definida ni validaciones de rango.

### Versión 2 (Prompt con Estructura y Restricciones)
```text
Actúa como desarrollador Java senior. Crea un programa estructurado en objetos para calcular el promedio de notas de un alumno. Usa una clase Alumno y una clase Curso. No utilices librerías externas.
```
* **Qué cambió y por qué:** Se añadió el **Rol** (desarrollador Java senior), más **Contexto** (clases Alumno y Curso) y una **Restricción** clara (no usar librerías externas) para estructurar el software.
* **Resultado de la IA:** El código ahora está orientado a objetos, pero la salida sigue siendo por consola y no valida si las notas ingresadas son correctas o negativas.

### Versión 3 (Prompt Profesional - Final)
```text
Actúa como desarrollador Java experto. Crea una aplicación de escritorio usando Java Swing para gestionar y calcular las notas de alumnos. 

Contexto: El sistema debe permitir ingresar el nombre del alumno y tres notas parciales.

Instrucción: Utiliza clases separadas para el modelo de datos y la interfaz gráfica. Valida que las notas estén estrictamente en el rango de 0 a 20. Si hay un error, muestra un mensaje emergente.

Restricciones: Usa únicamente los componentes nativos del JDK estándar (javax.swing.*).

Ejemplo de formato de salida:
Explica brevemente la arquitectura de las clases en viñetas y luego proporciona el código completo en un bloque limpio.
```
* **Qué cambió y por qué:** Se completaron de forma rigurosa los 5 componentes (Rol, Instrucción, Contexto, Restricciones y Formato) para tener el control total sobre la respuesta de la IA.
* **Resultado de la IA:** Se entrega una interfaz gráfica limpia con `JFrame`, cajas de texto, validaciones precisas y mensajes de error con `JOptionPane`.

---

## Anatomía del Prompt Final

| Componente | Texto exacto del prompt |
| :--- | :--- |
| **Rol** | Actúa como desarrollador Java experto. |
| **Instrucción** | Crea una aplicación de escritorio usando Java Swing para gestionar y calcular las notas... Utiliza clases separadas... Valida que las notas estén en el rango de 0 a 20. |
| **Contexto** | El sistema debe permitir ingresar el nombre del alumno y tres notas parciales. |
| **Restricciones** | Usa únicamente los componentes nativos del JDK estándar (javax.swing.*), sin librerías externas. |
| **Formato** | Explica brevemente la arquitectura de las clases en viñetas y luego proporciona el código completo. |

---

## Evaluación del Resultado

| Qué revisar | Cumple (Sí / No) |
| :--- | :--- |
| ¿Está escrito en Java y usa Swing de forma nativa? | Sí |
| ¿Permite ingresar los campos solicitados adecuadamente? | Sí |
| ¿Valida que las notas no salgan del rango de 0 a 20? | Sí |
| ¿Separa la lógica del modelo de la interfaz gráfica? | Sí |

---

## Errores Frecuentes Evitados

1. **Ser demasiado general (Falta de Formato):** Se evitó al definir en la versión 3 que el resultado requería viñetas explicativas antes del bloque de código.
2. **Asumir información no proporcionada:** En la primera versión la IA asumió una escala de notas del 0 al 100. Esto se corrigió especificando la escala local de 0 a 20.