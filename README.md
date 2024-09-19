# Base de datos de puntuación de crédito

Este repositorio contiene una base de datos en **SQLite3** diseñada para almacenar y gestionar información relacionada con el crédito. Los datos fueron recopilados por una empresa financiera global durante un año, e incluyen detalles bancarios básicos junto con información crediticia detallada con 100.000 registros.

## Descripción del conjunto de datos

- **Registros**: El conjunto de datos contiene 100,000 registros.
- **Características**: El conjunto de datos incluye 28 características que proporcionan información como:
  - Edad
  - Ocupación
  - Ingreso anual
  - Combinación de crédito
  - Número de préstamos
  - Puntuación de crédito
  - Antigüedad del historial crediticio
  - Ratio de utilización del crédito
  - Balance mensual, entre otros.

Cada cliente está representado por datos correspondientes a 8 meses consecutivos, lo que agrega un aspecto temporal para el análisis.

## Estructura de la base de datos

La base de datos está construida en **SQLite3** e incluye una vista, `credit_data_view`, que simplifica las consultas y la visualización de la información clave relacionada con el crédito. La vista integra datos de múltiples tablas, vinculando características como ocupación, combinación de crédito y tipos de préstamos con los detalles correspondientes de los clientes.

Las tablas clave incluyen:
- **credit_data_cod**: Contiene la información principal sobre crédito y banca para cada cliente.
- **ocupaciones**: Relaciona las ocupaciones de los clientes.
- **credit_mix**: Almacena información sobre el tipo de combinación de crédito.
- **loan**: Contiene los tipos de préstamos asociados a cada cliente.
- **payment_behaviour**: Registra el comportamiento de pago de cada individuo.
- **credit_score**: Almacena la categoría de puntuación de crédito.

La vista permite a los usuarios recuperar fácilmente una vista consolidada de los datos, incluyendo las puntuaciones de crédito de los clientes y su historial de préstamos.


- **Fuente de la informacion**: Kaggle - Dataset for Credit Score Classification
<!--  https://www.kaggle.com/datasets/ayushsharma0812/dataset-for-credit-score-classification/data
