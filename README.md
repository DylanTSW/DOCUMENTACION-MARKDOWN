# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Dylan Vazquez Soriano
## Actividad \#20
---

**DOCUMENTACIÓN DE OPERACIONES MATRICIALES APLICADAS A IMÁGENES EN EXCEL**

##  Archivo trabajado:

`tarea importante.xlsx`

---

##  **1. Objetivo**

El objetivo de este documento es explicar paso a paso el proceso de programación y aplicación de fórmulas en Microsoft Excel para manipular imágenes representadas como matrices numéricas de **30×30 píxeles**, aplicando conceptos básicos del álgebra matricial:

* Trasposición de matrices
* Multiplicación escalar
* Suma de matrices
* Resta de matrices
* Composición 

---

##  **2. Estructura del Archivo**

El archivo contiene **14 hojas**, divididas en:

* **5 hojas base:** imágenes originales en forma de matriz
* **5 hojas derivadas:** transpuestas de cada imagen
* **4 hojas de operaciones:** suma, resta, multiplicación escalar y composición 

La estructura general es la siguiente:


imagen 1

<img width="931" height="537" alt="image" src="https://github.com/user-attachments/assets/1bb4ef11-8660-4967-8274-d4de43b606af" />

Transpuesta 1

<img width="1109" height="661" alt="image" src="https://github.com/user-attachments/assets/1f3a4f14-85ac-49de-9f03-afb259b9558c" />

imagen 2

<img width="1077" height="630" alt="image" src="https://github.com/user-attachments/assets/0821a60d-e65d-4f89-9485-cc045b5d7d79" />

Transpuesta 2

<img width="989" height="567" alt="image" src="https://github.com/user-attachments/assets/6bc807cd-2de6-473f-870e-a660cd2d0628" />

Imagen 3

<img width="1193" height="653" alt="image" src="https://github.com/user-attachments/assets/c9bc71e0-d193-4e93-9fcb-49bcf30e6f73" />

Transpuesta 3

<img width="806" height="478" alt="image" src="https://github.com/user-attachments/assets/78dac6fd-d766-44a0-96cd-be17ba886a3f" />

imagen 4

<img width="1086" height="628" alt="image" src="https://github.com/user-attachments/assets/0d220d03-98cb-4ca0-a552-049dbae9e310" />

Transpuesta 4

<img width="1092" height="637" alt="image" src="https://github.com/user-attachments/assets/75773f01-149a-47af-8fbd-0c41a718b446" />

imagen 5

<img width="840" height="510" alt="image" src="https://github.com/user-attachments/assets/85738252-f67f-4634-933b-acec2a0f1a95" />

Transpuesta 5

<img width="779" height="446" alt="image" src="https://github.com/user-attachments/assets/e429df72-9309-4f8d-8473-721c8d397705" />

Suma

<img width="928" height="538" alt="image" src="https://github.com/user-attachments/assets/6b6a1839-8906-4e18-b833-2d2f585aa690" />

Resta

<img width="1139" height="658" alt="image" src="https://github.com/user-attachments/assets/5a3b5ae8-8d18-42f1-a9ee-3a52547d4840" />

Multiplicacion Escalar

<img width="895" height="508" alt="image" src="https://github.com/user-attachments/assets/a62dc7e5-83d2-4734-97b2-a2cc0b6ba82a" />

Composicion 

<img width="780" height="447" alt="image" src="https://github.com/user-attachments/assets/23b5b886-8ed9-47bc-a688-5b53ad7df236" />

---

##  **3. Documentación de las Hojas Base**

## ##  **3.1 Imágenes Originales**

Cada una contiene una **matriz 30×30** correspondiente a una imagen pixelada.
Cada celda contiene un valor (0, 1 o 2) que representa un color o intensidad.
Estas matrices servirán como base para todas las operaciones posteriores.

---

##  **4. Documentación de Matrices Transpuestas**

## ##  **4.1 Definición Matemática**

La traspuesta de una matriz ( A ) se define como:

Intercambia filas por columnas.

## ##  **4.2 Fórmula usada en Excel**

```
=TRANSPONER('imagen X'!A1:AD30)
```

**Instrucciones:**

1. Seleccionar un rango 30×30 vacío.
2. Escribir la fórmula.
3. Confirmar con Ctrl
4. Excel generará automáticamente la matriz traspuesta.

---

##  **5. Operaciones Matriciales**

Estas operaciones se encuentran en las siguientes hojas, aqui es donde realizamos las operaciones con dos imagenes que creamos:

* `Suma`
* `Resta`
* `Multiplicacion Escalar`
* `Composicion` 

La fórmula se arrastra hasta cubrir la matriz completa.

---

##  **5.2 Suma de Matrices**

### Fórmula en Excel

Ejemplo sumando `imagen 1` + `imagen 2`:

```
='imagen 1'!A1 + 'imagen 2'!A1
```

Se arrastra sobre 30×30 celdas.

---

##  **5.3 Resta de Matrices**

###  Fórmula en Excel

Ejemplo restando `imagen 1` - `imagen 2`:

```
='imagen 1'!A1 - 'imagen 2'!A1
```

También se arrastra sobre la matriz completa.

---

---

##  **5.1 Multiplicación Escalar**

### Fórmula en Excel

Si el escalar ( k ) está en la celda `B1` y la matriz base es `imagen 1`, entonces en `A1` colocamos:

```
='imagen 1'!A1 * $B$1
```


 ## **5.4 Composición Lineal**
 
###  Fórmula en Excel

```
=MMUL('imagen 1'!A1 * $B$1, 'imagen 2'!A1 * $B$2)
```

Arrastrar la fórmula hasta completar 30 filas × 30 columnas.

---
