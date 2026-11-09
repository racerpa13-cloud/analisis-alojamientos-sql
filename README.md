# Análisis y selección de alojamientos turísticos con SQL

## 1. Descripción del proyecto

Este proyecto analiza un conjunto de 20 alojamientos turísticos con el objetivo de identificar las propiedades que cumplen los requisitos de un cliente y recomendar la alternativa más adecuada.

El análisis parte de un caso práctico en el que un cliente busca alojamiento para ocho personas, con unas condiciones específicas de equipamiento, ubicación, precio y valoración. Mediante consultas SQL se relacionan diferentes tablas, se aplican los criterios de selección y se comparan las propiedades resultantes.

## 2. Objetivos

- Preparar los datos para su análisis mediante SQL.
- Identificar los alojamientos que cumplen los requisitos establecidos.
- Integrar información sobre características, ubicación, precios y puntuaciones.
- Comparar las alternativas seleccionadas y justificar una recomendación basada en datos.
- Explorar las características generales del catálogo mediante consultas complementarias.

## 3. Metodología

El proyecto se desarrolla en tres fases:

**Fase 1. Preparación de datos**

Revisión de las tablas, normalización de separadores decimales, conversión de tipos de datos, tratamiento de valores vacíos y eliminación de columnas adicionales generadas durante la importación.

**Fase 2. Análisis y selección de alojamientos**

Aplicación individual de los requisitos del cliente mediante consultas SQL. Posteriormente, integración de las cuatro tablas mediante `INNER JOIN` para aplicar conjuntamente todas las condiciones y seleccionar las propiedades que las cumplen.

**Fase 3. Análisis complementario y recomendación**

Comparación de las propiedades seleccionadas y elaboración de una recomendación basada en sus características y las necesidades del cliente. Se realizan consultas adicionales sobre superficie, equipamiento, distribución geográfica, precios y puntuaciones de las agencias.

## 4. Principales resultados

- **Cuatro alojamientos** cumplen todos los requisitos establecidos por el cliente.
- **Málaga** presenta la mayor superficie entre las alternativas seleccionadas (120 m²), con cuatro habitaciones, tres baños y una puntuación de 4,90.
- Frente a **Ibiza**, la otra alternativa con cuatro habitaciones, Málaga ofrece 20 m² adicionales, un baño más, una puntuación superior y un precio 100 € inferior por noche.
- La distribución de cuatro habitaciones y tres baños permite alojar a las ocho personas con mayor comodidad.

## 5. Conclusiones y limitaciones

El análisis permite identificar los alojamientos que cumplen las condiciones del cliente y recomendar la propiedad de Málaga por su combinación de superficie, capacidad, valoración y precio.

El proyecto muestra la utilidad de SQL para integrar información, aplicar criterios de selección y fundamentar decisiones a partir de datos.

Como limitación, el análisis se basa en un catálogo de 20 alojamientos y en los requisitos específicos de un único cliente. Por tanto, los resultados permiten seleccionar la mejor alternativa dentro de las propiedades disponibles, pero no establecer conclusiones generales sobre el mercado turístico.

## 6. Fuentes de datos

El proyecto utiliza cuatro archivos CSV proporcionados como parte de un ejercicio académico:

- `ALOJAMIENTO.csv`: características y equipamiento de las propiedades.
- `UBICACION.csv`: localización y distancias al metro y al centro.
- `PRECIO.csv`: precios de alquiler y porcentajes de reserva.
- `PUNTUACION.csv`: valoraciones de alojamientos y agencias.

Los cuatro conjuntos de datos se relacionan mediante el identificador `CODIGO_ALOJAMIENTO`.
