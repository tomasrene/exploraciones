# Vinos entre catálogos

Buscar joyitas entre catálogos de distribuidores y armar una carta de vinos.

Tenía un bar de vinos, Flama, y los distribuidores tenían catálogos que iban modificando y actualizando. Algunos eran larguísimos. Yo quería poder armar una carta a partir de los vinos que tenían los distintos distribuidores, encontrando joyitas o cosas que tuvieran que ver con el perfil del bar.

Además quería sacar toda la información: región, productor, cepas, añada, perfil, precio, etcétera. Ese era el problema real: tengo muchos catálogos, quiero buscar con criterio y armar una lista de vinos.

## “Quiero un tinto catalán ligero”

Los problemas técnicos eran dos. Por un lado, las búsquedas eran relativamente específicas: “quiero un tinto catalán ligero”. Para entender qué es un vino ligero y cuál puede serlo hace falta algo más que encontrar palabras parecidas en un catálogo.

Quería que el LLM pudiera razonar sobre lo que estaba pidiendo y los vinos disponibles. Después había que buscar en los catálogos y tener información suficiente para hacer esa selección.

## PDFs y Excels

Por otro lado estaban los formatos. Algunos catálogos eran Excel, otros PDFs estructurados, otros no estructurados. Había que explorar cómo trabajar con cada tipo de archivo y cómo llevar todos esos datos a un objeto con un mismo esquema.

Lo que armé fue una forma de resolver esos problemas: definí un objeto para representar los vinos, extraje la información mediante distintas técnicas —texto, OCR y llamadas a VLM, modelos que pueden leer las páginas como imágenes— y monté una mezcla de RAG con búsqueda de LLM encima.

Después había problemas como que el precio en algunos catálogos venía con IVA, en otros sin IVA, pero no estaba aclarado. En fin, problemas del mundo real.

- **La ficha del vino:** Región, productor, cepas, añada, perfil y precio, reunidos en un esquema común.
- **El precio también hay que leerlo:** En algunos catálogos venía con IVA, en otros sin IVA, y a veces ni siquiera estaba aclarado.

[Leer en la web](https://tomasrene.com/experimentos/vinos) · [Volver al catálogo](../README.md)
