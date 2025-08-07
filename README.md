# Alura Store Latam – Análisis de Ventas

Este repositorio contiene el cuaderno **`AluraStoreLatam.ipynb`** que analiza el desempeño de cuatro tiendas de la cadena *Alura Store* en Latinoamérica a partir de datos abiertos en CSV. El objetivo es obtener indicadores rápidos de facturación, ventas por categoría, satisfacción de clientes y logística.

## Tabla de contenido

1. [Descripción del proyecto](#descripción-del-proyecto)
2. [Estructura del notebook](#estructura-del-notebook)
3. [Requisitos](#requisitos)
4. [Instalación](#instalación)
5. [Uso](#uso)
6. [Conjunto de datos](#conjunto-de-datos)
7. [Resultados destacados](#resultados-destacados)
8. [Contribuciones](#contribuciones)
9. [Licencia](#licencia)
10. [Autor](#autor)

## Descripción del proyecto

El cuaderno realiza un **análisis exploratorio ligero (EDA)** para responder a preguntas clave de negocio:

* ¿Cuál es la **facturación total** de cada tienda?
* ¿Qué **categorías de productos** generan más ingresos?
* ¿Cuál es la **calificación promedio** otorgada por los clientes?
* ¿Qué productos son los **más y menos vendidos**?
* ¿Cuál es el **costo de envío promedio** por tienda?

Las respuestas se calculan únicamente con **Python y *pandas***, lo que hace que el proyecto sea fácil de reproducir y extender.

## Estructura del notebook

| Sección                           | Contenido                                                                    |
| --------------------------------- | ---------------------------------------------------------------------------- |
| 1. Importación de datos           | Lectura de cuatro archivos CSV con transacciones individuales.               |
| 2. Análisis de facturación        | Suma de ingresos por tienda y cálculo de un nuevo campo `Total_Facturación`. |
| 3. Ventas por categoría           | Agrupación (`groupby`) para ver ingresos por categoría de producto.          |
| 4. Calificación promedio          | Media simple de la columna `Calificación`.                                   |
| 5. Productos más / menos vendidos | Ranking de artículos según facturación acumulada.                            |
| 6. Envío promedio                 | Promedio de `Costo de envío` por tienda.                                     |

## Requisitos

* Python ≥ 3.8
* pandas
* jupyterlab o notebook clásico

*(Todas las dependencias están listadas en `requirements.txt` si decides agregarlo.)*

## Instalación

```bash
# 1. Clonar el repositorio
git clone https://github.com/<tu-usuario>/AluraStoreLatam.git
cd AluraStoreLatam

# 2. (Opcional) Crear y activar un entorno virtual
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# 3. Instalar dependencias
pip install -r requirements.txt  # o simplemente: pip install pandas jupyter
```

## Uso

1. Ejecuta `jupyter notebook` o `jupyter lab`.
2. Abre **`AluraStoreLatam.ipynb`**.
3. Ejecuta las celdas de arriba hacia abajo. Cada bloque imprime los indicadores calculados.

## Conjunto de datos

Los CSV provienen de URLs públicas de GitHub Raw (incluidas en la primera celda). Cada archivo contiene, entre otros, los siguientes campos:

* `Precio`
* `Cantidad de cuotas`
* `Categoría del Producto`
* `Calificación`
* `Costo de envío`

## Resultados destacados

* **Facturación total:** muestra el rendimiento global de cada tienda.
* **Top 5 categorías:** identifica las unidades de negocio más rentables.
* **Calificación promedio:** proxy de satisfacción del cliente.
* **Productos estrella y de baja rotación:** guía para decisiones de inventario.
* **Envío promedio:** indica posibles oportunidades de optimización logística.

## Contribuciones

¡Se aceptan *pull requests*! Por favor crea un branch, describe tu cambio y abre la PR.

## Licencia

Este proyecto se distribuye bajo la licencia MIT. Consulta el archivo `LICENSE` para más detalles.

## Autor

**Joanna Alexandra Carrión Pérez** – [@tu‑usuario](https://github.com/tu-usuario)

---

*Si te resulta útil, no olvides darle ⭐ al repositorio.*
