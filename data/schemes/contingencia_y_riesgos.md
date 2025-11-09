# Contingencia y Riesgos

## Riesgo 1 — Falla del pipeline nocturno / datos incompletos
**Señales:** faltan archivos, conteos inconsistentes, errores de ejecución.  
**Plan:**  
1) Reintento manual.
2) Validar conteos por tabla/fecha (test en `tests/`).  
3) Usar snapshot anterior y recalcular incrementales.  
4) Notificar a BI/DS sobre el desfase para evitar usar datos corruptos.

## Riesgo 2 — Cambios/Ruptura de esquema (tipos/columnas)
**Señales:** columnas nuevas/eliminadas, tipos distintos.  
**Plan:**  
1) Tests de contrato en Bronce; castear/normalizar en Silver.  
2) Versionar el diccionario de datos y comunicar cambios.  
4) Parche temporal en BI (medidas alternativas) hasta estabilizar el flujo.

## Riesgo 3 — Desempeño insuficiente del modelo
**Señales:** MAE/R² por debajo del umbral.  
**Plan:**  
1) Revisar features, outliers y fuga de datos.  
2) Probar modelos alternos.  
3) Ajustar ventana temporal y granularidad.  
4) Fallback: utilizar métricas descriptivas y reglas simples para la entrega.
