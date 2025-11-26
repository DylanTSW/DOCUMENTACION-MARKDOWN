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

```
imagen 1
Transpuesta 1
imagen 2
Transpuesta 2
Imagen 3
Transpuesta 3
imagen 4
Transpuesta 4
imagen 5
Transpuesta 5
Suma
Resta
Multiplicacion Escalar
Composicion 
```

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

### ✦ Fórmula en Excel

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
