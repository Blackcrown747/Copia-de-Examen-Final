# ⚙️ Scripts de Ingestión y EDA Mínimo (Capa BRONCE)

Este directorio contiene los scripts esenciales para la fase de **Ingestión y Estructuración (BRONCE)** del proyecto. Su función principal es garantizar que los datos brutos (`raw/`) sean cargados correctamente y que se realice una verificación inicial de su calidad antes de cualquier procesamiento.

---

## 1. `upload_cli.sh` – Carga de Datos Raw
Este script de Shell se utiliza para la automatización de la carga de archivos de datos brutos a la ubicación de almacenamiento persistente (Azure).


### 🎯 Propósito
* Garantizar la ingesta del archivo(s) (CSV) en el directorio `../bronce/raw/`.
* Registrar la operación de carga (si el comando CLI genera logs).
* Mantener la trazabilidad del proceso de ingesta.
