# Herramientas para restaurantes

Revisar las facturas de un bar y probar los números de un obrador de pasta.

Son dos herramientas que salieron de situaciones bastante distintas. Flama era mi bar de vinos y necesitaba revisar la contabilidad. Falcone era un proyecto de obrador de pasta que finalmente no llegamos a montar.

## Flama: revisar todas las facturas

Al revisar los borradores de IVA que nos pasaba la gestoría encontrábamos errores una y otra vez. En una ocasión la diferencia fue de cientos de euros, que para un bar es mucha plata.

Así que había que procesar todas las facturas de los proveedores y hacer las cuentas por nuestra cuenta para poder contrastarlas con el borrador. Ahí apareció otra vez el problema de los archivos: PDFs, imágenes, formatos distintos y datos repartidos de maneras bastante diferentes.

La herramienta salió de esa necesidad: extraer la información de las facturas, ordenarla y compararla con los registros de compras. El trabajo incluía revisar lo extraído contra el documento original.

## Falcone: jugar con los escenarios antes de abrir

Con Falcone quería construir una herramienta para jugar con escenarios de horarios, aforo y cubiertos servidos. Ver cómo cambiaban los números al mover unas pocas variables y dimensionar lo apretados que pueden ser los márgenes en gastronomía.

El simulador permite variar ventas, precios, costos de comida, trabajo y gastos fijos. El proyecto del obrador finalmente no se hizo; quedó esta herramienta para explorar qué pasaría si cambiara alguno de esos supuestos.

```python
gross_profit = total_revenue - total_food_cost
ebitda = gross_profit - labor_total - fixed_cost_total
```

Dos líneas de compute_pnl, la función que calcula los escenarios del simulador.

Eso era lo que quería mostrar: lo apretados que son los números en la gastronomía. Con una o dos variables que no controles, se te va todo a la mierda.

[Leer en la web](https://tomasrene.com/experimentos/restaurantes) · [Volver al catálogo](../README.md)

[Simulador de restaurante · código](https://github.com/tomasrene/simulador-restaurante) · [Facturas de restaurante · código](https://github.com/tomasrene/facturas-restaurante)
