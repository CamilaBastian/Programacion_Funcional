# ☕ Trabajo Práctico: Java Streams & Programación Funcional

![Java](https://img.shields.io/badge/Java-17%2B-orange?style=flat-square&logo=openjdk)
![Paradigm](https://img.shields.io/badge/Paradigm-Functional-blue?style=flat-square)
![UTN](https://img.shields.io/badge/UTN-Sistemas-blueviolet?style=flat-square)

> **Contexto Académico:**
> * **Ingeniería en Sistemas de Información:** Asignatura *Desarrollo de Software*.
> * **Tecnicatura Universitaria en Programación:** Asignatura *Programación III*.
>
> **Institución:** Universidad Tecnológica Nacional (UTN).

## 🎯 Objetivo General
Aplicar el paradigma funcional en Java utilizando la **Stream API** para el procesamiento declarativo de colecciones. El objetivo es reemplazar la iteración imperativa (bucles `for`/`while`) por pipelines de operaciones intermedias y terminales, mejorando la legibilidad y mantenibilidad del código.

---

## 📚 Marco Teórico y Competencias

En este proyecto se ponen en práctica los siguientes conceptos clave:

| Concepto | Aplicación Práctica |
|----------|---------------------|
| **Stream Pipeline** | Flujo de datos que permite transformaciones encadenadas (`map`, `filter`, `sorted`). |
| **Lambda Expressions** | Funciones anónimas para comportamientos concisos `(a -> a.getNota() > 7)`. |
| **Collectors** | Operaciones terminales para agrupar, sumarizar y transformar resultados. |
| **Inmutabilidad** | Enfoque en no modificar las colecciones originales, sino generar nuevos resultados. |
| **Method Reference** | Uso de `Clase::metodo` para un código más limpio. |

---

## 🛠 Casos Prácticos Implementados

El repositorio contiene la resolución de 4 escenarios de negocio distintos, simulando requerimientos de reportes y análisis de datos.

### 🎓 Caso 1: Gestión Académica (Clase `Alumno`)
*Dominio:* `Alumno(nombre, nota, curso)`
1.  **Filtrado y Transformación:** Obtener nombres de alumnos aprobados (nota ≥ 7) en mayúsculas y ordenados.
2.  **Reducción:** Calcular el promedio general de notas del curso.
3.  **Agrupamiento:** Agrupar alumnos por curso (`Collectors.groupingBy`).
4.  **Ranking:** Obtener los 3 mejores promedios.

### 📦 Caso 2: Inventario y Stock (Clase `Producto`)
*Dominio:* `Producto(nombre, categoria, precio, stock)`
1.  **Ordenamiento:** Listar productos caros (>100) ordenados descendentemente.
2.  **Agrupamiento Complejo:** Agrupar por categoría y sumar el stock total (`summingInt`).
3.  **Formato de Salida:** Generar reporte en String separando productos por `";"` (`Collectors.joining`).
4.  **Estadísticas:** Calcular precio promedio general y por categoría.

### 📚 Caso 3: Biblioteca (Clase `Libro`)
*Dominio:* `Libro(titulo, autor, paginas, precio)`
1.  **Filtrado Complejo:** Libros extensos (>300 págs) ordenados alfabéticamente.
2.  **Cálculo:** Promedio de páginas totales.
3.  **Conteo:** Agrupar por autor y contar cantidad de obras (`Collectors.counting`).
4.  **Máximos:** Encontrar el libro más costoso de la colección (`Comparator.comparing`).

### 💼 Caso 4: Recursos Humanos (Clase `Empleado`)
*Dominio:* `Empleado(nombre, departamento, salario, edad)`
1.  **Filtro y Orden:** Empleados con salario > 2000, orden descendente.
2.  **Estadística:** Salario promedio de la empresa.
3.  **Sumatoria:** Agrupar por departamento y calcular el gasto total en salarios (`summingDouble`).
4.  **Límites:** Obtener los 2 empleados más jóvenes (`sorted` + `limit`).

---

## 🚀 Cómo Ejecutar el Proyecto

Este proyecto es una aplicación de consola estándar de Java.

1.  **Clonar el repositorio:**
    ```bash
    git clone [https://github.com/TU-USUARIO/tp-functional-streams.git](https://github.com/TU-USUARIO/tp-functional-streams.git)
    ```
2.  **Importar en IDE:**
    Abrir el proyecto en **IntelliJ IDEA**, **Eclipse** o **NetBeans**.
3.  **Ejecución:**
    Cada caso práctico se encuentra en su propia clase `Main` o método de prueba. Ejecutar la clase principal correspondiente para ver la salida en consola.

---

## 📝 Conclusiones de Aprendizaje

El desarrollo de este TP permitió consolidar la transición del pensamiento imperativo al declarativo. Se verificó cómo los **Streams** reducen la complejidad ciclomática del código, eliminando bucles anidados y variables temporales, facilitando la lectura y la generación de estadísticas complejas con pocas líneas de código.

---

## 👤 Autor

**Nombre:** Camila Bastian
**Legajo:** 50795
**Materia:** Desarrollo de Software

```
