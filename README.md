# libreria
### Repositorio de Biblioteca

Este repositorio contiene un sistema de gestión para una biblioteca, implementado en Python. El sistema permite administrar clientes, libros y ventas, así como generar estadísticas relacionadas con las ventas. A continuación, se describen las principales funcionalidades del sistema:

#### Funcionalidades Principales

1. **Gestión de Clientes**
   - Ingresar nuevos clientes.
   - Actualizar información de clientes existentes.
   - Listar todos los clientes.
   - Borrar clientes (siempre que no tengan ventas registradas).
   - Buscar clientes por código.

2. **Gestión de Libros**
   - Ingresar nuevos libros.
   - Actualizar cantidad de unidades disponibles.
   - Actualizar precios de libros.
   - Listar todos los libros disponibles.
   - Borrar libros (siempre que no tengan ventas registradas).
   - Buscar libros por código.

3. **Gestión de Ventas**
   - Registrar nuevas ventas.
   - Listar todas las ventas realizadas.
   - Buscar ventas por código.
   - Actualizar detalles de ventas.
   - Borrar ventas.

4. **Estadísticas**
   - Ventas totales de libros por ISBN.
   - Identificar el libro más vendido y el menos vendido.
   - Calcular la venta total de la librería.
   - Identificar el cliente con mayor compra por venta.
   - Identificar el cliente con mayor volumen de compra total.

#### Ejemplo de Uso

##### Gestión de Clientes
```python
# Ingresar un nuevo cliente
ingresar_clientes()

# Listar todos los clientes
lista_clientes()

# Actualizar un cliente
actualizar_cliente()

# Borrar un cliente
borrar_cliente()

# Buscar un cliente
buscar_cliente()
```

##### Gestión de Libros
```python
# Ingresar un nuevo libro
ingreso_libros()

# Listar todos los libros
lista_libros()

# Actualizar cantidad de libros
actualizar_cantidad()

# Actualizar precio de un libro
actualizar_precio()

# Borrar un libro
borrar_libro()

# Buscar un libro
buscar_libro()
```

##### Gestión de Ventas
```python
# Registrar una nueva venta
registrar_venta()

# Listar todas las ventas realizadas
mostrar_ventas()

# Buscar una venta
buscar_venta_menu()

# Actualizar una venta
actualizar_venta()

# Borrar una venta
borrar_ventas()
```

##### Estadísticas
```python
# Ventas totales de libros por ISBN
obtener_ventas_totales_por_codigo_libro()

# Libro más y menos vendido
mostrar_libros_mas_y_menos_vendido()

# Venta total de la librería
calcular_venta_total_libreria()

# Cliente con mayor compra por venta
obtener_cliente_con_mayor_compra_por_venta()

# Cliente con mayor volumen de compra total
obtener_cliente_con_mayor_volumen_compra_total()
```

#### Estructura de Datos

- **Clientes**: Lista de listas, donde cada sublista contiene el nombre y el código del cliente.
```python
clientes = [
    ["juan", 3100],
    ["maria", 3101],
    ["pedro", 3102],
    ["laura", 3103]
]
```

- **Libros**: Lista de listas, donde cada sublista contiene el código, nombre, precio y unidades disponibles del libro.
```python
libros = [
    [12552, "iliada", 5300, 25],
    [12553, "platero", 2500, 16],
    [12554, "cien", 3600, 35]
]
```

- **Ventas**: Lista de tuplas, donde cada tupla contiene el código de la venta, código del cliente, código del libro, cantidad vendida y valor de la venta.
```python
ventas = [
    (1020, 3100, 12552, 4, 21200),
    (1025, 3102, 12553, 2, 5000),
    (1030, 3100, 12554, 3, 10800),
    (1035, 3101, 12553, 9, 22500)
]
```

#### Requisitos
- Python 3.x

#### Cómo Ejecutar
1. Clone este repositorio.
2. Ejecute el archivo principal para iniciar el menú interactivo:
```sh
python biblioteca.py
```
