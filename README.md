
# Proyecto Analítica — Repositorio Base

## Equipos y Tareas

### Data Engineering (DE)
- Ingestar los CSV (`data/raw/` → Bronce).
- Crear pipelines y staging SQL.
- Limpieza inicial, tipificación y control de calidad.
- Cargar datos a Fabric / Lakehouse.
- Automatizar procesos de actualización.

### Business Analytics (BA)
- Analizar variables dependientes e independientes.
- Ejecutar queries SQL / Python para correlaciones.
- Validar consistencia de datos y KPIs.
- Generar reportes para BI y DS.

### Business Intelligence (BI)
- Crear modelo de datos en Power BI (`bi/dashboards/`).
- Diseñar medidas DAX (`bi/dax/`).
- Desarrollar dashboards interactivos y segmentadores.
- Entregar análisis visual final.

### Data Science (DS)
- Modelar variable dependiente (`SalesAmount`).
- Entrenar y validar modelos predictivos.
- Guardar artefactos (`data/models/`).
- Desarrollar app (`scripts/app/`) para visualizar resultados.

## Uso
1. Coloca los CSV en `data/raw/` (ya incluidos).
2. Documenta scripts en `scripts/` según la capa.
3. Guarda resultados intermedios en `data/cleaned/` o `data/outputs/`.
4. Crea notebooks temáticos en `notebooks/`.
5. Sube diagramas e informes a `docs/`.
