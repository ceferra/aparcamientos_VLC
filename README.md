# aparcamientos_VLC — Ocupación de aparcamientos (València)

Archivo histórico de la **ocupación de los aparcamientos públicos** de
València (plazas totales y libres), del portal de datos abiertos municipal
(hoy descatalogado).

## Origen

- **Fuente:** Ayuntamiento de València — portal *mapas.valencia.es*
  (`lanzadera/opendata/Tra-aparcamientos/CSV`).
- Servicio descatalogado; este repositorio es la copia de respaldo del
  histórico.

## Periodo

- **1149 días** entre **09-09-2019** y **24-10-2024**.

## Estructura del repositorio

- Un fichero ZIP por día: `DD-MM-YYYY.zip`, con los CSV capturados ese día.
- Un commit ("new day") por día, fechado con la fecha real del dato.

## Formato y campos

Ficheros **CSV** con separador `;`. Columnas:

| Columna      | Significado                                              |
|--------------|---------------------------------------------------------|
| `X`, `Y`     | Coordenadas del aparcamiento en **UTM EPSG:25830**.     |
| `nombre`     | Nombre del aparcamiento.                                 |
| `direccion`  | Dirección postal.                                        |
| `numeropol`  | Número de policía (portal).                              |
| `tipo`       | Tipo de aparcamiento.                                    |
| `plazastota` | Plazas totales.                                          |
| `plazaslibr` | Plazas libres en el momento de la captura. `-1` = sin dato. |
