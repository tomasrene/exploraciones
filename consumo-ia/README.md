# Medir el consumo de IA

Entender la cuota, los tokens y el costo estimado de las herramientas.

**Estado: en pruebas.**

## Qué quería hacer

Quiero entender cuánto estoy usando las herramientas de IA y qué significa cada número. La cuota de una cuenta, los tokens registrados localmente y un costo estimado responden preguntas distintas.

## Qué probé

Armé un monitor local con historial y un tablero por fechas y modelos. Consulta la cuota e importa contadores de tokens sin guardar el texto de las conversaciones.

También estima un equivalente de costo por API con tarifas verificadas y muestra qué parte del uso puede valorar. Esa estimación no es una factura ni el precio de la suscripción.

## Tres números diferentes

| Medida | Qué cuenta |
| --- | --- |
| Cuota | La ventana de uso informada por la cuenta. |
| Tokens locales | Los eventos registrados en este equipo. |
| Costo estimado | Una valoración con tarifas de API y cobertura explícita. |

## Qué sigue abierto

Cómo mostrar lo que se pudo medir sin dar una falsa impresión de cobertura total: puede haber uso desde otros equipos o servicios que no aparece en el registro local.

[Leer en la web](https://tomasrene.com/experimentos/consumo-ia) · [Volver al catálogo](../README.md)
