# 📚 Análisis de Algoritmos

Repositorio educativo que contiene **notebooks interactivos** y **análisis teóricos** sobre diseño y análisis de algoritmos. Este material está diseñado para estudiantes de la materia **Diseño y Análisis de Algoritmos** (5º semestre).

---

## 📋 Contenido del Repositorio

### 🔍 **Conceptos Fundamentales**

#### 1. **Factorial_Iterativo_vs_Recursivo.ipynb**
Comparación experimental entre implementaciones iterativa y recursiva del factorial.
- Implementación de `factorial_iterativo()` y `factorial_recursivo()`
- Medición de tiempos de ejecución
- Identificación del límite de recursión en Python (≈977)
- Análisis del costo de control vs aritmética de enteros grandes
- **Conceptos:** Recursión, profundidad de llamadas, pila (call stack)

#### 2. **Fibonacci:comparación_iterativo_vs_recursivo.ipynb**
Análisis experimental de Fibonacci con múltiples enfoques.
- Fibonacci recursivo ingenuo (crecimiento exponencial)
- Conteo de llamadas y iteraciones
- Visualización de subproblemas traslapados
- **Conceptos:** O(2ⁿ), subestructura óptima, recomputación

---

### 🧠 **Estructuras de Datos y Búsqueda**

#### 3. **Algoritmos_Basados_en_Grafos.ipynb**
Exploración de algoritmos fundamentales en grafos.
- **BFS (Búsqueda por Anchura):** O(V + E), búsqueda de camino mínimo
- **DFS (Búsqueda por Profundidad):** O(V + E), exploración, detección de ciclos
- **Backtracking:** Construcción de árbol de decisiones, problema de N-Reinas
- Comparación conceptual entre estrategias
- **Conceptos:** Recorridos, exploración, validación, poda

---

### 🎯 **Estrategias de Diseño**

#### 4. **Divide_and_Conquer.ipynb**
Estrategia fundamental de Divide y Vencerás.
- **Merge Sort:** O(n log n), aplicación de Divide y Vencerás
- **Bubble Sort:** O(n²), referencia de algoritmo clásico
- **Binary Search:** O(log n), búsqueda binaria
- Método Maestro para análisis de recurrencias
- Validación experimental vs referencias teóricas
- **Conceptos:** Recurrencias, T(n) = aT(n/b) + f(n), notación asintótica

#### 5. **Estrategias_Greedy.ipynb**
Algoritmos greedy con enfoque en selección de actividades.
- Implementación de `seleccion_actividades_greedy()`
- Validación contra fuerza bruta para instancias pequeñas
- Justificación de decisiones locales óptimas
- Análisis experimental de rendimiento
- **Conceptos:** Decisiones locales, subestructura óptima, O(n log n)

#### 6. **Programacion_dinamica.ipynb** y **programacion_dinamica.ipynb**
Técnicas de Programación Dinámica.
- **Fibonacci con memoización y tabulación**
- **Corte de varillas:** maximización de ingresos
- **Problema de la Mochila 0/1** (en archivo separado)
- Comparación: recursivo ingenuo vs top-down vs bottom-up
- **Conceptos:** Subestructura óptima, subproblemas traslapados, O(n²)

#### 7. **Programacion_dinamica.ipynb** (Mochila 0/1)
Resolución completa del problema clásico de optimización.
- `knapsack_recursive()` - versión recursiva sin PD
- `knapsack_top_down()` - memoización
- `knapsack_bottom_up()` - tabulación
- Validación con 10,000 instancias de Kaggle
- Comparación experimental de rendimiento
- **Conceptos:** O(n×W), recuperación de soluciones, optimización

---

### 📊 **Análisis Experimental**

#### 8. **Analisis_experimental_de_complejidad.ipynb**
Medición práctica de complejidad temporal.
- **Búsqueda lineal:** O(n) en peor caso
- **BogoSort:** O(n!), crecimiento factorial
- Mejor caso vs peor caso vs caso promedio
- Visualización en escala logarítmica
- **Conceptos:** Empirismo vs teoría, ruido experimental

#### 9. **Analisis_experimental_de_rendimiento_(Cocktail_Sort_vs_Bubble_Sort).ipynb**
Comparación de dos algoritmos de ordenamiento.
- Implementación de `bubble_sort()` y `cocktail_sort()`
- Medición en: entrada aleatoria, ordenada, inversa
- Análisis de escala log vs lineal
- Identificación de tendencias experimentales
- **Conceptos:** O(n²), mejora marginal, early stopping

---

## 🎓 Temas Cubiertos

| Tema | Archivos | Complejidad |
|------|----------|-------------|
| Recursión | Factorial, Fibonacci | Varía |
| Búsqueda | BFS, DFS, Binary Search | O(n), O(V+E), O(log n) |
| Ordenamiento | Bubble, Cocktail, Merge | O(n²), O(n log n) |
| Divide y Vencerás | Merge Sort, Binary Search | O(n log n), O(log n) |
| Greedy | Selección de Actividades | O(n log n) |
| Programación Dinámica | Fibonacci, Mochila, Varillas | O(n), O(nW), O(n²) |
| Backtracking | N-Reinas | O(n!) |

---

## 🛠️ Tecnologías y Herramientas

- **Lenguaje:** Python 3
- **Entorno:** Google Colab
- **Librerías principales:**
  - `time` / `perf_counter()` - medición de tiempos
  - `matplotlib` - visualización
  - `pandas` - manejo de datos
  - `functools.lru_cache` - memoización
  - `kagglehub` - carga de datasets

---

## 🚀 Cómo Usar

### Opción 1: Google Colab (Recomendado)
Haz clic en el botón "Open in Colab" dentro de cada notebook para ejecutar directamente sin instalación.

### Opción 2: Local
```bash
# Clonar repositorio
git clone https://github.com/AlexanderOlivera/Analisis-de-algoritmos.git

# Instalar dependencias
pip install -r requirements.txt

# Ejecutar Jupyter
jupyter notebook
```

### Opción 3: Descargar archivos
Descarga los `.ipynb` individualmente y ábrelos con Jupyter Notebook o JupyterLab.

---

## 📝 Estructura de Cada Notebook

Cada notebook incluye típicamente:

1. **Descripción teórica** - Concepto, definiciones, notación asintótica
2. **Implementación** - Código completo con comentarios
3. **Validación** - Pruebas de correctitud (sanity check)
4. **Experimento** - Medición de tiempos para distintos tamaños `n`
5. **Gráficas** - Visualización de comportamiento experimental
6. **Análisis** - Interpretación de resultados y preguntas de reflexión

---

## 📐 Notación Asintótica

| Notación | Interpretación | Ejemplo |
|----------|---|---|
| O(1) | Tiempo constante | Acceso a array |
| O(log n) | Logarítmico | Binary Search |
| O(n) | Lineal | Búsqueda lineal |
| O(n log n) | Lineal-logarítmico | Merge Sort |
| O(n²) | Cuadrático | Bubble Sort |
| O(n³) | Cúbico | Floyd-Warshall |
| O(2ⁿ) | Exponencial | Fibonacci naive |
| O(n!) | Factorial | Backtracking, N-Reinas |

---

## ❓ Preguntas de Reflexión por Tema

### Recursión vs Iteración
- ¿Qué ventajas y desventajas tiene cada enfoque?
- ¿Cuál es el costo oculto en la recursión?

### BFS vs DFS
- ¿Cuándo usar cada uno?
- ¿Qué garantías ofrece BFS en grafos no ponderados?

### Divide y Vencerás
- ¿Qué propiedades debe cumplir el problema?
- ¿Cómo aplica el Método Maestro?

### Greedy
- ¿Por qué funciona la decisión local?
- ¿Cómo se demuestra optimalidad?

### Programación Dinámica
- ¿Qué diferencia hay entre top-down y bottom-up?
- ¿Cuál es el espacio vs tiempo?

---

## 🎯 Objetivos de Aprendizaje

Al completar estos notebooks, serás capaz de:

✅ Analizar la complejidad temporal y espacial de algoritmos  
✅ Distinguir entre diferentes paradigmas de diseño  
✅ Justificar decisiones algorítmicas con evidencia experimental  
✅ Implementar soluciones eficientes con múltiples enfoques  
✅ Interpretar gráficas de rendimiento  
✅ Demostrar correctitud de algoritmos  
✅ Aplicar técnicas avanzadas (DP, Greedy, Backtracking)

---

## 📚 Referencias y Recursos

- **CLRS:** "Introduction to Algorithms" (Cormen, Leiserson, Rivest, Stein)
- **Skiena:** "Algorithm Design Manual"
- **MIT OpenCourseWare:** Algorithms
- **Documentación oficial:** Python, NumPy, Matplotlib

---

## 👤 Autor

**Alexander Olivera**  
Estudiante de Ingeniería en Sistemas Computacionales

---

## 📄 Licencia

Este repositorio está bajo licencia **MIT**. Siéntete libre de usar, modificar y distribuir el contenido con atribución.

---

## 💬 Contribuciones

¿Encontraste un error o tienes una mejora? 
- Abre un **Issue**
- Crea un **Pull Request**
- Comparte feedback constructivo

---

## 📧 Contacto

Para preguntas o sugerencias:
- **GitHub Issues:** [Abre aquí](https://github.com/AlexanderOlivera/Analisis-de-algoritmos/issues)
- **Discusiones:** [Participa en las discusiones](https://github.com/AlexanderOlivera/Analisis-de-algoritmos/discussions)

---

**Última actualización:** 2026-05-08  
**Versión:** 1.0
