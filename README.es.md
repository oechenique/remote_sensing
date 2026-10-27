# remote_sensing — resumen en español

[🇬🇧 English](README.md)

Teledetección con Python en tres notebooks que corren en Colab o en local, sin bajar imágenes a mano, sin cuenta y sin GPU:

1. **Bosques del mundo**: el mapa de cobertura arbórea de Global Map (~1 km) con estadísticas ponderadas por área. El 23 % de la tierra al norte de 60°S está bajo copa.
2. **Sentinel-2 sobre Antalya por STAC**: búsqueda con `pystac-client`, carga lazy con `odc-stac`, máscara de nubes con SCL, compuesto mensual sin nubes y NDVI con `spyndex`.
3. **Incendio de Manavgat (2021)**: severidad con dNBR (~50.000 ha quemadas, 22.300 de severidad alta o moderada-alta) y la recuperación 2019–2026. Cinco años después el bosque quemado recuperó el 60 % de la diferencia con un bosque sano de control.

Lo más interesante del camino: la Collection 1 de Sentinel-2 casi no tiene 2022 en esa zona. Además, la colección vieja que llena el hueco publica un offset en su metadata que sus píxeles ya no tienen; aplicarlo deformaba la serie. Los notebooks originales de 2023–2024 quedan en `legacy/`.
