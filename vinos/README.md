# Vinos entre catálogos

Buscar joyitas entre catálogos de distribuidores y armar una carta de vinos.

Cuando tenía Flama, un bar de vinos, quería armar la carta a partir de lo que ofrecían los distintos distribuidores. Encontrar joyitas, vinos que tuvieran que ver con el perfil del bar, y reunir la información para elegir: región, productor, cepas, añada, perfil y precio.

El problema era que tenía muchos catálogos. Algunos larguísimos, que además se iban actualizando. Quería poder buscar con criterio y armar una lista sin tener que recorrerlos todos cada vez.

## “Quiero un tinto catalán ligero”

Ese es el tipo de pedido que quería poder hacer. La región puede estar escrita en el catálogo; “ligero” ya requiere interpretar qué vino podría encajar con lo que estoy buscando. Encontrar un fragmento de texto parecido no alcanza para resolver toda la consulta.

La exploración combinó recuperar información de los catálogos con un LLM que pudiera razonar sobre el pedido y los vinos disponibles.

## Antes había que leer los catálogos

Había Excels, PDFs bastante estructurados y otros donde el diseño complicaba sacar cualquier dato. Definí un objeto común para representar cada vino y fui probando distintas formas de llevar los catálogos a ese esquema: extracción de texto, OCR y modelos que leen imágenes y texto, los VLM.

Después monté una mezcla de RAG y búsqueda con LLM sobre esa información. La idea era poder pasar de todos esos archivos a una selección para la carta.

- **La ficha del vino:** Región, productor, cepas, añada, perfil y precio, reunidos en un esquema común.
- **El precio también hay que leerlo:** En algunos catálogos venía con IVA, en otros sin IVA, y a veces ni siquiera estaba aclarado.

Terminó siendo bastante más interesante técnicamente de lo que parecía al principio. Una búsqueda aparentemente sencilla obligaba a trabajar con formatos distintos, interpretar pedidos y resolver detalles tan poco vistosos como averiguar qué incluía un precio. Problemas del mundo real, básicamente.

[Leer en la web](https://tomasrene.com/experimentos/vinos) · [Volver al catálogo](../README.md)
