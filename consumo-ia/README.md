# Medir el consumo de IA

Un tablero para entender cuánto estoy usando las herramientas de IA.

Quería entender los números de uso: cuánto queda de cuota, cuántos tokens registra este equipo y qué costaría algo equivalente por API. Son medidas distintas y era fácil mezclarlas.

Armé un monitor local que guarda lecturas y un tablero por fechas y modelos. Importa contadores sin guardar el texto de las conversaciones. También calcula una estimación con tarifas de API cuando hay información suficiente.

El registro local no ve todo: puede faltar uso desde otro equipo o servicio. La cuota pertenece a la cuenta completa. Esa diferencia tiene que quedar visible para que el gráfico no cuente una historia que los datos no sostienen.

[Leer en la web](https://tomasrene.com/experimentos/consumo-ia) · [Volver al catálogo](../README.md)
