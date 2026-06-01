# Informe de Base de Datos

## 1. Descripción general
Esta base de datos sirve para gestionar la información de una empresa de venta de cocinas, incluyendo clientes, productos, compras e instalaciones. Permite controlar todo el proceso desde la compra hasta la instalación final.

## 2. Estructura
- Tablas:
  - cliente
  - cocinas
  - compras
  - instalacion
  - instaladores

- Relaciones:
  - Un cliente puede realizar varias compras
  - Cada compra está asociada a una cocina
  - Cada instalación está relacionada con una compra
  - Los instaladores realizan las instalaciones

## 3. Análisis
- Qué está bien diseñado:
  - Las relaciones entre tablas están bien definidas mediante claves foráneas
  - Existe integridad referencial entre clientes, compras e instalaciones

- Qué no está claro:
  - Algunos campos podrían tener mejor normalización
  - El campo de instalación podría separarse en más información detallada

## 4. Problemas detectados
- Algunos registros pueden tener valores por defecto poco claros
- Falta validación más estricta en algunos campos numéricos
- Algunas relaciones podrían ser más detalladas

## 5. Propuestas de mejora
- Crear una tabla de “pagos” para registrar métodos de pago
- Añadir una tabla de “proveedores” para las cocinas
- Mejorar la normalización separando direcciones en campos más pequeños
- Añadir más restricciones (NOT NULL, CHECK)

## 6. Conclusión personal
He aprendido a trabajar con bases de datos relacionales, a realizar consultas SQL, a entender las relaciones entre tablas y a estructurar un proyecto completo usando GitHub y MySQL.
