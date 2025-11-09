# Variables del Modelo

## Variable Dependiente (Target)
- **SalesAmount** — monto de venta por transacción (objetivo de predicción).

## Variables Independientes (Features)
- **SalesQuantity** — cantidad vendida.
- **DiscountQuantity** — unidades con descuento / intensidad de descuento.
- **UnitPrice** — precio unitario del producto.
- **PromotionKey / Campaign** — campaña promocional aplicada (si aplica).
- **ChannelKey / ChannelName** — canal de venta (Online, Store, etc.).
- **StoreType** — tipo de tienda.
- **Geography (Country, Region, ContinentName)** — localización del punto de venta.
- **Date features** — Year, Month, Quarter, Day, Weekday, IsWeekend, Season.
- **Product hierarchy** — Category, Subcategory, Brand.
- **Returns** — ReturnQuantity, ReturnAmount (si impactan el objetivo).
- **Variables derivadas** (ejemplos): precio neto, % descuento, ticket promedio por tienda/mes, estacionalidad.
