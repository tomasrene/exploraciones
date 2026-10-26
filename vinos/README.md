# Vinos entre catálogos

Reunir catálogos de distribuidores para buscar y comparar vinos.

**Estado: en pruebas.**

## Qué quería hacer

Quiero juntar catálogos de varios distribuidores y poder consultarlos en un mismo lugar. Los archivos llegan en PDFs y Excels, con estructuras y formas de presentar precios bastante distintas.

## Qué probé

Probé extracción de texto de PDF y una variante con OCR para recuperar información que aparece en imágenes, como algunos nombres de bodegas. Hay archivos estructurados resultantes de esas pruebas.

La búsqueda incluye comparar parsers, OCR y modelos que leen imágenes y texto. La integración entre distribuidores y la revisión de lo extraído siguen abiertas; los VLM son una herramienta a explorar, no una garantía de precisión.

## Lo que debería conservar una búsqueda

| Dato | Para qué sirve |
| --- | --- |
| Vino, bodega y añada | Distinguir referencias que se parecen. |
| Formato y precio | Comparar botellas y condiciones equivalentes. |
| Distribuidor y archivo de origen | Volver al catálogo cuando algo no cierra. |
| Fecha del catálogo | Saber si el precio puede haber cambiado. |

## Qué sigue abierto

Cómo reconocer el mismo vino entre catálogos, conservar la añada y el formato y saber de qué archivo y fecha salió cada precio.

[Leer en la web](https://tomasrene.com/experimentos/vinos) · [Volver al catálogo](../README.md)
