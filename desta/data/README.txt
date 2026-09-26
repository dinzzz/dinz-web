Desta OpenStreetMap-derived data — published 26 September 2026

© OpenStreetMap contributors. Adaptations by Dinzel IT d.o.o.
These databases are available under the Open Database Licence (ODbL) 1.0:
https://opendatacommons.org/licenses/odbl/1-0/
Any rights in individual contents of these databases are licensed under the
Database Contents License: https://opendatacommons.org/licenses/dbcl/1-0/
OSM attribution: https://www.openstreetmap.org/copyright

This download supplies the complete OSM-derived datasets used for the described
Desta functionality, without requiring a Desta account or payment.

osm-coastline-2026-05-31.json.gz: unmodified compressed Overpass source snapshot
for coastal exposure calculations. Database timestamp 2026-05-31T22:37:44Z;
3,625 natural=coastline ways in bounds south 41.9, west 12.8, north 46.0, east 19.0.
Decompressed SHA256: 30606e80285b0b5fe6c13af2e8d8be1a8feb37bbdd23dd2daa24761a28dc0224.

coastal-exposure.json: the complete 54-record derived estimate subset from the
build 9 catalogue, including per-direction values, sampling/origin metadata,
source date/hash and licence attribution. Harbour identifiers associate records
with the app. This download does not license unrelated publisher text or facts.
Desta computes coastal fetch and lower/moderate/higher exposure bands; these
are estimates rather than official shelter assessments.

sea_mask.bin and sea_meta.json: complete adapted sea/land grid used by the
backend's route search. It was generated from OSM coastline using rasterization
and flood fill. Its original source snapshot date is not established; do not
assign it the May 2026 exposure-snapshot date. Metadata supplies west, north,
dLon, dLat, cols, rows and rowBytes. Each row is rowBytes bytes; cell (col,row)
is sea when (bytes[row*rowBytes+(col>>3)] & (1<<(7-(col&7)))) is nonzero.
Cell centres: lon=west+(col+0.5)*dLon; lat=north-(row+0.5)*dLat.

These data are not nautical charts and establish neither safe navigation nor
under-keel clearance. See licence for warranty exclusions and reuse conditions.
Contact: dinz@dinzzz.com.
