# aparcamientos_VLC — Car-park occupancy (València)

Historical archive of **public car-park occupancy** (total and free spaces)
for València, from the municipal open-data portal (now decommissioned).

## Source

- **Publisher:** València City Council — *mapas.valencia.es* portal
  (`lanzadera/opendata/Tra-aparcamientos/CSV`).
- Decommissioned service; this repository is the backup copy of the history.

## Period

- **1149 days** between **2019-09-09** and **2024-10-24**.

## Repository layout

- One ZIP file per day: `DD-MM-YYYY.zip`, holding the CSVs captured that day.
- One commit ("new day") per day, dated with the real date of the data.

## Format and fields

**CSV** files with `;` separator. Columns:

| Column       | Meaning                                                  |
|--------------|----------------------------------------------------------|
| `X`, `Y`     | Car-park coordinates in **UTM EPSG:25830**.              |
| `nombre`     | Car-park name.                                            |
| `direccion`  | Postal address.                                           |
| `numeropol`  | Street number (door number).                              |
| `tipo`       | Car-park type.                                            |
| `plazastota` | Total spaces.                                             |
| `plazaslibr` | Free spaces at capture time. `-1` = no data.             |
