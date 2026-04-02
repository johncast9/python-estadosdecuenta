# Identificacion Ordenantes

Scripts en Python para consolidar archivos de Excel y generar la identificación de ordenantes a partir de descripciones de movimientos.

## Archivos

* script_concentrado.py: consolida múltiples archivos Excel
* script_referencias.py: analiza el concentrado y genera referencias

## Uso

1. Configurar rutas en los scripts:

```python
INPUT_FOLDER = "C:\\Ruta\\Entrada"
OUTPUT_FILE = "C:\\Ruta\\Salida\\Concentrado.xlsx"
```

```python
INPUT_FILE = "C:\\Ruta\\Entrada\\Concentrado.xlsx"
CUENTAS_FILE = "C:\\Ruta\\Entrada\\Cuentas.xlsx"
OUTPUT_FILE = "C:\\Ruta\\Salida\\Resultado.xlsx"
```

2. Ejecutar en orden:

```bash
python script_concentrado.py
python script_referencias.py
```

## Requisitos

```bash
pip install pandas openpyxl
```

## Notas

* Se requieren columnas como Fecha, Concepto y Monto
* Ajustar reglas según el formato de los archivos
* No incluir información sensible
