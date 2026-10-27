# Herramientas para restaurantes

Números, facturas y otras tareas alrededor de un restaurante.

Acá se juntan dos pruebas distintas. Una para jugar con los números de un negocio; otra para ordenar el trabajo de las facturas. Todavía no forman un sistema integrado.

## Falcone: mover un supuesto

Falcone es un simulador mensual. Se pueden mover ventas, precios, costos de comida, trabajo y gastos fijos para ver cómo cambia el resultado. Los valores son supuestos del modelo.

```python
gross_profit = total_revenue - total_food_cost
ebitda = gross_profit - labor_total - fixed_cost_total
```

Dos líneas de compute_pnl, la función que calcula los escenarios del simulador.

## Flama: del documento a la tabla

Flama arranca en otro lugar: facturas en PDF o imagen que hay que pasar a una tabla y revisar. Hay pruebas de extracción y comparación con registros de compras.

Me interesa que el dato extraído siga cerca del documento. Si algo no cierra, debería poder volver a la factura y corregirlo sin perder esa decisión en la próxima importación.

[Leer en la web](https://tomasrene.com/experimentos/restaurantes) · [Volver al catálogo](../README.md)

[Simulador de restaurante · código](https://github.com/tomasrene/simulador-restaurante) · [Facturas de restaurante · código](https://github.com/tomasrene/facturas-restaurante)
