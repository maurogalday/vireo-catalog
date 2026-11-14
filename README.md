# Catálogo de dispositivos de Vireo

Lista pública de dispositivos que reconoce [Vireo](https://github.com/maurogalday), la app para controlar
luces RGB, ventiladores y sensores de la PC.

- `catalog.json`: modelos y marcas (identificación USB o nombre, tipo, driver y funciones).
- `catalog.json.sig`: firma ECDSA P-256 (SHA-256). Vireo solo usa un catálogo descargado si la firma es
  válida y la versión es más nueva que la que trae integrada.

Para publicar una versión nueva: subir `version`, validar con `Vireo.CatalogTool check`, firmar con
`Vireo.CatalogTool sign` y subir los dos archivos.