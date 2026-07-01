# Academic Store Inventory

Sistema de gestión de productos para una tienda académica, desarrollado en Java como parte de la evaluación PA4 - Programación Orientada a Objetos.

## Objetivo

Diseñar e implementar una solución en Java que integre colecciones de objetos y una jerarquía de clases, aplicando herencia, clase abstracta, interfaz y sobrescritura de métodos, para registrar, almacenar y consultar productos de una tienda académica.

## Integrantes y matriz de participación

| Nombre | Correo | Rol / Módulo desarrollado | % de participación |
|---|---|---|---|
| Nombre Apellido 1 | correo1@isil.pe | Jerarquía de clases (Producto, subclases, interfaz) | 25% |
| Nombre Apellido 2 | correo2@isil.pe | Colecciones y unicidad (List, HashSet) | 25% |
| Nombre Apellido 3 | correo3@isil.pe | Búsqueda, ordenamiento y menú | 25% |
| Nombre Apellido 4 | correo4@isil.pe | Integración, pruebas, README y video | 25% |

## Descripción de la solución

El sistema permite registrar, listar, buscar y ordenar productos de una tienda académica. Se modeló una jerarquía de clases con:

- Producto (clase abstracta): define los atributos y comportamientos comunes a todos los productos.
- ProductoFisico y ProductoDigital (clases derivadas): representan tipos distintos de producto, cada una sobrescribiendo el método mostrarInfo().
- Descontable (interfaz): define el comportamiento obligatorio aplicarDescuento(), implementado por las clases de producto.

Para el almacenamiento se utilizó:
- Una colección genérica (List<Producto>) para registrar todos los productos.
- Un HashSet<String> para validar la unicidad del código de producto antes de registrarlo.

El sistema implementa además una búsqueda por código/nombre y un ordenamiento sobre la colección de productos.

## Decisiones técnicas tomadas por el equipo

(Completar: por qué eligieron esos dos tipos de producto, por qué esa clase abstracta, qué criterio usaron para el ordenamiento, etc.)

## Instrucciones de ejecución

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/usuario/academic-store-inventory.git
   ```
## Video de explicación

Enlace del video: (agregar enlace de YouTube aquí - cámaras encendidas, explicando cómo resolvieron la evaluación, por qué llegaron a esa solución y qué decisiones tomaron)

## Estructura del proyecto

```
academic-store-inventory/
├── src/
│   ├── Producto.java
│   ├── ProductoFisico.java
│   ├── ProductoDigital.java
│   ├── Descontable.java
│   ├── Inventario.java
│   └── Main.java
├── README.md
└── .gitignore
```

## Curso

Programación Orientada a Objetos - Evaluación PA4 (Sesión 13)
